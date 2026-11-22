# 🔬 GraphIDS — Flagship Case Studies

> highest-scoring TP / FN / FP in the test set · threshold **126.7** · scores are reconstruction error in GNN embedding space

## ✅ TP · TRUE POSITIVE — correctly flagged · `Exploits`

> **`175.45.176.2` → `149.171.126.16`** · score **379.8** vs threshold **126.7** (3.0× over)

**Strongest anomaly:** `MAX_TTL` at **358.5×** benign-typical error

| where the error lives | share |
|---|---:|
| src-context (GNN) | 2.5% |
| flow features (45) | 95.4% |
| dst-context (GNN) | 2.1% |

**Integrated Gradients (top 3):**

| # | feature | IG attribution | error × benign |
|---|---|---:|---:|
| 1 | `MAX_TTL` | +159.756 | 358.5× |
| 2 | `MIN_TTL` | +104.133 | 44.5× |
| 3 | `SHORTEST_FLOW_PKT` | +91.712 | 15.2× |

**Verdict:** detector right for the right reason — MAX_TTL dominates the attribution (358.5× benign-typical), the classic off-subnet TTL signature

---

## 🕳️ FN · FALSE NEGATIVE — missed attack · `Exploits`

> **`175.45.176.3` → `149.171.126.17`** · score **106.3** vs threshold **126.7** (84% of cutoff)

**Strongest anomaly:** `RETRANSMITTED_IN_BYTES` at **69.6×** benign-typical error

| where the error lives | share |
|---|---:|
| src-context (GNN) | 9.6% |
| flow features (45) | 79.5% |
| dst-context (GNN) | 10.9% |

**Integrated Gradients (top 3):**

| # | feature | IG attribution | error × benign |
|---|---|---:|---:|
| 1 | `RETRANSMITTED_IN_BYTES` | +30.163 | 69.6× |
| 2 | `IN_BYTES` | +29.900 | 51.7× |
| 3 | `RETRANSMITTED_IN_PKTS` | +23.429 | 14.5× |

**Verdict:** anomaly is real but sub-threshold — 20.4 points short (84% of the cutoff); signal lives in RETRANSMITTED_IN_BYTES, not the TTL channel that flags other Exploits

---

## ⚠️ FP · FALSE POSITIVE — false alarm · `Benign`

> **`59.166.0.3` → `149.171.126.8`** · score **677.8** vs threshold **126.7** (5.3× over)

**Strongest anomaly:** `DURATION_IN` at **103.8×** benign-typical error

| where the error lives | share |
|---|---:|
| src-context (GNN) | 0.4% |
| flow features (45) | 99.3% |
| dst-context (GNN) | 0.3% |

**Integrated Gradients (top 3):**

| # | feature | IG attribution | error × benign |
|---|---|---:|---:|
| 1 | `SERVER_TCP_FLAGS` | +65.334 | 96.8× |
| 2 | `DURATION_IN` | +63.377 | 103.8× |
| 3 | `SRC_TO_DST_IAT_MAX` | +58.697 | 22.4× |

**Verdict:** benign flow whose DURATION_IN rhythm mimics attack patterns — the FP cluster Phase 4 flags for threshold/whitelist tuning

---
