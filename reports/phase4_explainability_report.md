# Phase 4 Report — Explainability & LLM Narration


### Reproduction gate
Phase 4 re-derived the Phase 3 test set before explaining anything. Confusion matrix: TP 70,233 · FP 8,000 · FN 22,418 · TN 935,244 — exact match with Phase 3. PR-AUC 0.8074 · ROC-AUC 0.9813. All explanations apply to the exact evaluated model.  

### Explanation stack
1. Per-dim reconstruction error in GNN embedding space — z = [src-context 48 | flow 45 | dst-context 48]
2. Integrated Gradients (Captum, 32 steps) — 256 sampled TP/FN/FP/TN edges attributed to the 45 flow features
3. Aggregate forensics — per-class error heatmaps, error-block splits, FN/FP driver features
4. Flagship case studies — highest-scoring TP / FN / FP with verdicts
5. LLM SOC alerts — 36 narrations, 34 valid, 81% automated faithfulness; severity dashboard


### Findings

- **Exploit misses:** detected Exploits carry MAX_TTL error 300–358× benign-typical; missed Exploits 4.7–7.6× — a ~50× separation confirming the TTL "hidden label" effect documented for UNSW-NB15.False
- **positives:** one coherent cluster — SRC_TO_DST_IAT_AVG, DURATION_IN/OUT, SERVER_TCP_FLAGS. Largest explainable FP: OSPF multicast 10.40.182.1 → 224.0.0.5 (IAT error 435×) — whitelisting candidate.
- **Analysis class:** error split 20/62/18 (src/flow/dst) vs ~4/92/4 elsewhere — benign-looking features on atypical node pairs.
- **Faithfulness:** 81% mean (LLM cited model-attributed features); real feature names recovered from scaler.feature_names_in_ and fingerprint-verified (ordering A: ports kept, timestamps dropped).

### Artifacts
phase4_summary.json · phase4_figures.png · phase4_alerts.json · phase4_narration.md · phase4_cases.md · explain_samples.json
