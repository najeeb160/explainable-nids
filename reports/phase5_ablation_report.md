# Phase 5 Report — No-TTL Ablation Study

## Motivation

Phase 4's Integrated-Gradients forensics found that every detected attack edge carried an anomalous TTL signature (MAX_TTL reconstruction error 300–358× benign-typical) while missed attacks lacked it (4.7–7.6×) — consistent with the documented UNSW-NB15 caveat that TTL acts as a hidden label. A finding from explainability is a hypothesis until tested; this ablation tests it.

### Design
Identical protocol to Phase 3 — seed 42, same temporal split, same architecture, benign-only training, early stopping on val PR-AUC (patience 20), threshold = p99 of benign validation errors — with one controlled change: MIN_TTL and MAX_TTL removed (45 → 43 flow features). The model was retrained from scratch (83,755 parameters; 35 epochs, early stop; best val PR-AUC 0.3407 vs 0.7988 with TTL). No LLM narration by design — the deliverable is the controlled comparison.

### Results

| Metric | With TTL | No TTL | Δ |
| :--- | :---: | :---: | :---: |
| Validation PR-AUC | 0.7988 | 0.3407 | −0.458 |
| Test PR-AUC | 0.8074 | 0.3322 | −0.475 |
| ROC-AUC | 0.9813 | 0.8885 | −0.093 |
| Val F1 @ p95 | 0.765 | 0.425 | −0.340 |
| Test F1 @ p99 (protocol rule) | 0.8220 | 0.0246 | −0.797 |

Per-class test recall (w/ TTL → no TTL): Fuzzers 98.2% → 0.7% · Worms 97.5% → 5.0% · Reconnaissance 91.5% → 1.1% · Generic 90.5% → 1.4% · Shellcode 89.7% → 0.3% · Backdoor 79.6% → 1.7% · DoS 69.1% → 3.0% · Exploits 47.9% → 1.8% · Analysis 1.4% → 0.4%.

### Findings
1. **Universal collapse** — every class loses >66 recall points except the already-failing Analysis class; TTL carried nearly all discriminative signal.
2. **Ranking survives, separability dies** — ROC-AUC drops only 0.09 while threshold detection collapses. Without TTL, the attack score distribution (val mean 35.6) sits below the benign 99th percentile (223.7): the populations overlap so heavily that no practical threshold exists. Threshold-robust conclusion: even the best validation operating point (p95) yields validation F1 0.425 vs 0.765 with TTL under the identical rule.
3. **Prediction → confirmation** — IG attributions identified TTL as the dominant driver of correct detections before the ablation; the controlled experiment quantified its worth.

### Interpretation
TTL is both a testbed artifact (simulated off-subnet attackers carry distinctive TTL values) and a trivially spoofable feature in adversarial settings. Under either reading, the reported F1 = 0.822 must be interpreted with this dependency explicit — and it would have remained invisible without the explainability stack. Attribution analysis therefore functions as a diagnostic instrument for benchmark validity, not merely alert decoration.

### Artifacts
graphids_model_nottl.pt · phase5_ablation_summary.json · phase5_figures.png
