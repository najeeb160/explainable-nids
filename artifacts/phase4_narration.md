# 🛡️ GraphIDS — SOC Alert Narratives

> **36** narrations · faithfulness **84%** · threshold **126.7**

## 📊 Dashboard

| # | Type | Label | Flow | Score | Severity |
|---|------|-------|------|------:|----------|
| 01 | 🚨 alert | Fuzzers | `175.45.176.0` → `149.171.126.13` | 205.8 | 🟠 high |
| 02 | 🚨 alert | Fuzzers | `175.45.176.3` → `149.171.126.14` | 201.2 | 🟠 high |
| 03 | 🚨 alert | Fuzzers | `175.45.176.1` → `149.171.126.11` | 312.5 | 🟠 high |
| 04 | 🚨 alert | Fuzzers | `175.45.176.1` → `149.171.126.15` | 232.4 | 🟠 high |
| 05 | 🚨 alert | Exploits | `175.45.176.3` → `149.171.126.10` | 217.8 | 🟠 high |
| 06 | 🚨 alert | Generic | `175.45.176.3` → `149.171.126.18` | 243.3 | 🟠 high |
| 07 | 🚨 alert | Exploits | `175.45.176.1` → `149.171.126.14` | 229.1 | 🟠 high |
| 08 | 🚨 alert | Reconnaissance | `175.45.176.2` → `149.171.126.16` | 233.2 | 🟠 high |
| 09 | 🚨 alert | Generic | `175.45.176.1` → `149.171.126.14` | 260.8 | 🟠 high |
| 10 | 🚨 alert | Fuzzers | `175.45.176.1` → `149.171.126.15` | 244.6 | 🟠 high |
| 11 | 🚨 alert | Generic | `175.45.176.2` → `149.171.126.11` | 231.3 | 🔴 critical |
| 12 | 🚨 alert | Reconnaissance | `175.45.176.3` → `149.171.126.11` | 219.7 | 🟠 high |
| 13 | 🚨 alert | Fuzzers | `175.45.176.3` → `149.171.126.14` | 360.8 | 🟠 high |
| 14 | 🚨 alert | Exploits | `175.45.176.3` → `149.171.126.10` | 211.0 | 🟠 high |
| 15 | 🚨 alert | Exploits | `175.45.176.3` → `149.171.126.13` | 209.7 | 🟠 high |
| 16 | 🚨 alert | Benign | `59.166.0.4` → `149.171.126.7` | 500.7 | 🟠 high |
| 17 | 🚨 alert | Benign | `59.166.0.1` → `149.171.126.2` | 281.3 | 🟠 high |
| 18 | 🚨 alert | Benign | `59.166.0.1` → `149.171.126.3` | 388.1 | 🟠 high |
| 19 | 🚨 alert | Benign | `59.166.0.7` → `149.171.126.9` | 165.8 | 🟠 high |
| 20 | 🚨 alert | Benign | `59.166.0.4` → `149.171.126.7` | 460.2 | 🟠 high |
| 21 | 🚨 alert | Benign | `59.166.0.8` → `149.171.126.1` | 278.3 | 🟠 high |
| 22 | 🚨 alert | Benign | `59.166.0.9` → `149.171.126.2` | 387.0 | 🟠 high |
| 23 | 🚨 alert | Benign | `59.166.0.1` → `149.171.126.0` | 268.3 | 🟠 high |
| 24 | 🚨 alert | Benign | `10.40.182.1` → `224.0.0.5` | 398.6 | 🟠 high |
| 25 | 🚨 alert | Benign | `59.166.0.3` → `149.171.126.7` | 400.4 | 🟠 high |
| 26 | 🚨 alert | Benign | `59.166.0.9` → `149.171.126.6` | 393.6 | 🟠 high |
| 27 | 🚨 alert | Benign | `59.166.0.2` → `149.171.126.9` | 137.9 | 🟠 high |
| 28 | 🚨 alert | Benign | `59.166.0.9` → `149.171.126.2` | 211.5 | 🟠 high |
| 29 | 🚨 alert | Benign | `59.166.0.1` → `149.171.126.8` | 459.0 | 🟠 high |
| 30 | 🚨 alert | Benign | `59.166.0.0` → `149.171.126.2` | 132.1 | 🟠 high |
| 31 | 🕳️ missed | Exploits | `175.45.176.0` → `149.171.126.10` | 17.4 | 🕳️ gap |
| 32 | 🕳️ missed | Exploits | `175.45.176.3` → `149.171.126.10` | 19.6 | 🕳️ gap |
| 33 | 🕳️ missed | Exploits | `175.45.176.3` → `149.171.126.19` | 41.0 | 🕳️ gap |
| 34 | 🕳️ missed | Reconnaissance | `175.45.176.3` → `149.171.126.13` | 23.7 | 🕳️ gap |
| 35 | 🕳️ missed | Generic | `175.45.176.3` → `149.171.126.15` | 22.2 | 🕳️ gap |
| 36 | 🕳️ missed | Reconnaissance | `175.45.176.2` → `149.171.126.18` | 17.9 | 🕳️ gap |

---

## 🚨 01 · 🟠 **HIGH** · `Fuzzers`

> **175.45.176.0 → 149.171.126.13** · score **205.8** vs threshold **126.7**

**Severity:** high — Unusual TTL drop 🚨  
**What happened:** 175.45.176.0 → 149.171.126.13  
**Why flagged:** MAX_TTL = 9.165, 321x benign-typical error; MIN_TTL = 9.153, 43.5x benign-typical error  
**Behaviour hypothesis:** consistent with a stealthy ICMP probe attempting to bypass normal TTL thresholds.  
**Recommended action:** Block ICMP traffic from 175.45.176.0 and monitor for repeat TTL anomalies.

| feature | value (z) | error × benign | IG attribution |
|--------:|----------:|---------------:|---------------:|
| `MAX_TTL` | 9.165 | 321.0× | +97.428 |
| `MIN_TTL` | 9.153 | 43.5× | +96.444 |
| `LONGEST_FLOW_PKT` | 1.256 | 0.4× | -3.744 |
| `MIN_IP_PKT_LEN` | -1.61 | 0.3× | +2.737 |
| `ICMP_TYPE` | 1.981 | 0.1× | -2.733 |

---

## 🚨 02 · 🟠 **HIGH** · `Fuzzers`

> **175.45.176.3 → 149.171.126.14** · score **201.2** vs threshold **126.7**

**Severity:** high — *TTL anomaly detected 🚨*  
**What happened:** 175.45.176.3 → 149.171.126.14  
**Why flagged:** MIN_TTL = 9.153, 43.5x benign‑typical error; MAX_TTL = 9.165, 317.9x benign‑typical error; DST_TO_SRC_IAT_AVG = 1.657, 1.8x benign‑typical error.  
**Behaviour hypothesis:** consistent with a low‑TTL stealth scan attempting to evade detection.  
**Recommended action:** block source IP 175.45.176.3 and investigate related traffic for port‑scanning activity.

| feature | value (z) | error × benign | IG attribution |
|--------:|----------:|---------------:|---------------:|
| `MIN_TTL` | 9.153 | 43.5× | +95.197 |
| `MAX_TTL` | 9.165 | 317.9× | +84.570 |
| `MIN_IP_PKT_LEN` | -1.61 | 0.3× | +3.602 |
| `MAX_IP_PKT_LEN` | -1.039 | 0.0× | -3.184 |
| `DST_TO_SRC_IAT_AVG` | 1.657 | 1.8× | +2.505 |

---

## 🚨 03 · 🟠 **HIGH** · `Fuzzers`

> **175.45.176.1 → 149.171.126.11** · score **312.5** vs threshold **126.7**

**Severity:** high — Unusual TTL drop detected 🚨  
**What happened:** 175.45.176.1 → 149.171.126.11  
**Why flagged:** MAX_TTL = 9.123, 349.1x benign-typical error; MIN_TTL = 9.153, 41.2x error; SHORTEST_FLOW_PKT = 10.0, 14.1x error  
**Behaviour hypothesis:** consistent with a potential TTL‑manipulating stealth scan.  
**Recommended action:** isolate the source host and perform a packet capture for deeper analysis.

| feature | value (z) | error × benign | IG attribution |
|--------:|----------:|---------------:|---------------:|
| `MAX_TTL` | 9.123 | 349.1× | +109.037 |
| `MIN_TTL` | 9.153 | 41.2× | +101.311 |
| `SHORTEST_FLOW_PKT` | 10.0 | 14.1× | +84.502 |
| `MIN_IP_PKT_LEN` | -5.857 | 2.5× | +11.963 |
| `SRC_TO_DST_AVG_THROUGHPUT` | 4.295 | 2.6× | +4.275 |

---

## 🚨 04 · 🟠 **HIGH** · `Fuzzers`

> **175.45.176.1 → 149.171.126.15** · score **232.4** vs threshold **126.7**

**Severity:** high — Unusual TTL drop detected 🚨  
**What happened:** 175.45.176.1 → 149.171.126.15  
**Why flagged:** MAX_TTL = 9.165, 320x benign-typical error; MIN_TTL = 9.153, 45.7x error  
**Behaviour hypothesis:** consistent with a misconfigured or malicious device sending packets with abnormally low TTL values.  
**Recommended action:** Verify the source host’s routing configuration and inspect for potential compromise.

| feature | value (z) | error × benign | IG attribution |
|--------:|----------:|---------------:|---------------:|
| `MAX_TTL` | 9.165 | 320.0× | +111.383 |
| `MIN_TTL` | 9.153 | 45.7× | +95.792 |
| `MIN_IP_PKT_LEN` | -1.61 | 0.3× | +4.720 |
| `DST_TO_SRC_IAT_AVG` | 2.928 | 6.5× | +3.997 |
| `DST_TO_SRC_AVG_THROUGHPUT` | -0.629 | 0.0× | -2.927 |

---

## 🚨 05 · 🟠 **HIGH** · `Exploits`

> **175.45.176.3 → 149.171.126.10** · score **217.8** vs threshold **126.7**

**Severity:** high — *Anomalous TTL burst 🚨*  
**What happened:** 175.45.176.3 → 149.171.126.10  
**Why flagged:** MAX_TTL = 9.165, 326.1x benign-typical error; MIN_TTL = 9.153, 43.6x error; RETRANSMITTED_IN_BYTES = 1.844, 6.3x error  
**Behaviour hypothesis:** consistent with a misconfigured or malicious host sending packets with unusually low TTL values.  
**Recommended action:** isolate the source IP and perform a packet capture to verify TTL manipulation and potential exfiltration.

| feature | value (z) | error × benign | IG attribution |
|--------:|----------:|---------------:|---------------:|
| `MAX_TTL` | 9.165 | 326.1× | +98.627 |
| `MIN_TTL` | 9.153 | 43.6× | +89.974 |
| `RETRANSMITTED_IN_BYTES` | 1.844 | 6.3× | +4.282 |
| `RETRANSMITTED_IN_PKTS` | 1.743 | 1.2× | +4.016 |
| `MIN_IP_PKT_LEN` | -1.61 | 0.2× | +3.047 |

---

## 🚨 06 · 🟠 **HIGH** · `Generic`

> **175.45.176.3 → 149.171.126.18** · score **243.3** vs threshold **126.7**

**Severity:** high — “Unusual TTL drop, suspicious traffic 🚨”  
**What happened:** 175.45.176.3 → 149.171.126.18  
**Why flagged:** MAX_TTL = 9.123, 357.8x benign-typical error; MIN_TTL = 9.153, 41.4x benign-typical error; DNS_QUERY_TYPE = 4.433, 1.0x benign-typical error  
**Behaviour hypothesis:** consistent with a compromised host attempting to evade detection by manipulating TTL values.  
**Recommended action:** isolate the source IP, block outbound traffic to the destination, and conduct a forensic packet capture.

| feature | value (z) | error × benign | IG attribution |
|--------:|----------:|---------------:|---------------:|
| `MAX_TTL` | 9.123 | 357.8× | +111.496 |
| `MIN_TTL` | 9.153 | 41.4× | +94.980 |
| `DNS_QUERY_TYPE` | 4.433 | 1.0× | +26.644 |
| `L4_SRC_PORT` | -1.665 | 0.2× | -4.334 |
| `TCP_FLAGS` | -1.822 | 2.4× | +4.163 |

---

## 🚨 07 · 🟠 **HIGH** · `Exploits`

> **175.45.176.1 → 149.171.126.14** · score **229.1** vs threshold **126.7**

**Severity:** high — Unusual TTL drop, suspicious traffic 🚨  
**What happened:** 175.45.176.1 → 149.171.126.14  
**Why flagged:** MAX_TTL = 9.123, 332.3x benign-typical error; MIN_TTL = 9.153, 41.3x benign-typical error; TCP_FLAGS = -1.822, 2.6x benign-typical error  
**Behaviour hypothesis:** consistent with a stealthy scanning or tunneling attempt.  
**Recommended action:** isolate the source host and block outbound traffic to 149.171.126.14.

| feature | value (z) | error × benign | IG attribution |
|--------:|----------:|---------------:|---------------:|
| `MAX_TTL` | 9.123 | 332.3× | +109.718 |
| `MIN_TTL` | 9.153 | 41.3× | +101.504 |
| `MIN_IP_PKT_LEN` | -5.857 | 1.8× | +5.999 |
| `L4_SRC_PORT` | -1.327 | 0.2× | -3.411 |
| `TCP_FLAGS` | -1.822 | 2.6× | +2.784 |

---

## 🚨 08 · 🟠 **HIGH** · `Reconnaissance`

> **175.45.176.2 → 149.171.126.16** · score **233.2** vs threshold **126.7**

**Severity:** high — Unusual TTL drop, suspicious traffic 🚨  
**What happened:** 175.45.176.2 → 149.171.126.16  
**Why flagged:** MAX_TTL = 9.123, 327.9x benign-typical error; MIN_TTL = 9.153, 42.4x benign-typical error; TCP_FLAGS = -1.822, 2.4x benign-typical error  
**Behaviour hypothesis:** consistent with a stealthy probe attempting to evade detection by manipulating TTL values.  
**Recommended action:** isolate the source host and conduct a packet capture to verify malicious intent.

| feature | value (z) | error × benign | IG attribution |
|--------:|----------:|---------------:|---------------:|
| `MAX_TTL` | 9.123 | 327.9× | +117.792 |
| `MIN_TTL` | 9.153 | 42.4× | +106.305 |
| `TCP_FLAGS` | -1.822 | 2.4× | +3.756 |
| `L7_PROTO` | -1.216 | 1.7× | +3.260 |
| `ICMP_IPV4_TYPE` | -1.187 | 0.0× | -2.877 |

---

## 🚨 09 · 🟠 **HIGH** · `Generic`

> **175.45.176.1 → 149.171.126.14** · score **260.8** vs threshold **126.7**

**Severity:** high — anomalous TTL behavior 🚨  
**What happened:** 175.45.176.1 → 149.171.126.14  
**Why flagged:** MAX_TTL = 9.123, 348x benign-typical error; MIN_TTL = 9.153, 43x benign-typical error  
**Behaviour hypothesis:** consistent with TTL spoofing or misconfigured host attempting to evade detection.  
**Recommended action:** Immediately block 175.45.176.1 at the perimeter firewall.

| feature | value (z) | error × benign | IG attribution |
|--------:|----------:|---------------:|---------------:|
| `MAX_TTL` | 9.123 | 348.0× | +109.540 |
| `MIN_TTL` | 9.153 | 43.2× | +101.544 |
| `DNS_QUERY_TYPE` | 4.433 | 1.1× | +28.115 |
| `MIN_IP_PKT_LEN` | -5.857 | 2.2× | +4.895 |
| `TCP_FLAGS` | -1.822 | 4.2× | +4.813 |

---

## 🚨 10 · 🟠 **HIGH** · `Fuzzers`

> **175.45.176.1 → 149.171.126.15** · score **244.6** vs threshold **126.7**

**Severity:** high — Unusual TTL, high retransmissions 🚨  
**What happened:** 175.45.176.1 → 149.171.126.15  
**Why flagged:** MAX_TTL = 9.165, 328x benign-typical error; MIN_TTL = 9.153, 44.7x error; RETRANSMITTED_IN_BYTES = 3.418, 21.6x error  
**Behaviour hypothesis:** consistent with a misconfigured or malicious host repeatedly retransmitting packets with abnormally low TTLs.  
**Recommended action:** isolate the source IP and perform packet capture to verify legitimate traffic or block if malicious.

| feature | value (z) | error × benign | IG attribution |
|--------:|----------:|---------------:|---------------:|
| `MAX_TTL` | 9.165 | 328.0× | +108.713 |
| `MIN_TTL` | 9.153 | 44.7× | +96.961 |
| `RETRANSMITTED_IN_BYTES` | 3.418 | 21.6× | +12.436 |
| `RETRANSMITTED_IN_PKTS` | 2.919 | 4.9× | +8.876 |
| `IN_BYTES` | 3.381 | 15.3× | +7.142 |

---

## 🚨 11 · 🔴 **CRITICAL** · `Generic`

> **175.45.176.2 → 149.171.126.11** · score **231.3** vs threshold **126.7**

**Severity:** critical — extreme TTL anomaly 🚨  
**What happened:** 175.45.176.2 → 149.171.126.11  
**Why flagged:** MAX_TTL = 9.123, 336.7x benign-typical error; MIN_TTL = 9.153, 42.2x error  
**Behaviour hypothesis:** consistent with a mis‑configured or malicious host sending packets with unusually low TTL values.  
**Recommended action:** isolate the source IP, block outbound traffic, and investigate host configuration.

| feature | value (z) | error × benign | IG attribution |
|--------:|----------:|---------------:|---------------:|
| `MAX_TTL` | 9.123 | 336.7× | +110.950 |
| `MIN_TTL` | 9.153 | 42.2× | +98.148 |
| `MIN_IP_PKT_LEN` | -5.857 | 2.2× | +8.063 |
| `TCP_FLAGS` | -1.639 | 2.1× | +4.046 |
| `L7_PROTO` | -1.216 | 2.9× | +3.842 |

---

## 🚨 12 · 🟠 **HIGH** · `Reconnaissance`

> **175.45.176.3 → 149.171.126.11** · score **219.7** vs threshold **126.7**

**Severity:** high — Unusual TTL drop detected 🚨  
**What happened:** 175.45.176.3 → 149.171.126.11  
**Why flagged:** MAX_TTL = 9.165, 316.4x benign-typical error; MIN_TTL = 9.153, 42.9x benign-typical error; DST_TO_SRC_IAT_AVG = 5.642, 32.3x benign-typical error  
**Behaviour hypothesis:** consistent with a low‑TTL stealth scan attempting to evade detection.  
**Recommended action:** block the source IP and monitor for repeated low‑TTL probes.

| feature | value (z) | error × benign | IG attribution |
|--------:|----------:|---------------:|---------------:|
| `MAX_TTL` | 9.165 | 316.4× | +102.202 |
| `MIN_TTL` | 9.153 | 42.9× | +96.894 |
| `DST_TO_SRC_IAT_AVG` | 5.642 | 32.3× | +14.154 |
| `DST_TO_SRC_IAT_MAX` | 1.661 | 0.1× | -2.969 |
| `DST_TO_SRC_IAT_STDDEV` | 3.951 | 3.5× | -2.535 |

---

## 🚨 13 · 🟠 **HIGH** · `Fuzzers`

> **175.45.176.3 → 149.171.126.14** · score **360.8** vs threshold **126.7**

**Severity:** high — suspicious TTL anomaly 🚨  
**What happened:** 175.45.176.3 → 149.171.126.14  
**Why flagged:** MAX_TTL = 9.123, 352x benign-typical error; MIN_TTL = 9.153, 43.1x error; SHORTEST_FLOW_PKT = 10.0, 14.9x error  
**Behaviour hypothesis:** consistent with a misconfigured or malicious device manipulating TTL values.  
**Recommended action:** isolate the source host and perform a packet capture to verify TTL manipulation.

| feature | value (z) | error × benign | IG attribution |
|--------:|----------:|---------------:|---------------:|
| `MAX_TTL` | 9.123 | 352.0× | +132.535 |
| `MIN_TTL` | 9.153 | 43.1× | +106.773 |
| `SHORTEST_FLOW_PKT` | 10.0 | 14.9× | +90.516 |
| `MIN_IP_PKT_LEN` | -5.857 | 2.5× | +7.431 |
| `PROTOCOL` | 1.558 | 1.7× | +4.333 |

---

## 🚨 14 · 🟠 **HIGH** · `Exploits`

> **175.45.176.3 → 149.171.126.10** · score **211.0** vs threshold **126.7**

**Severity:** high — Unusual TTL drop detected 🚨  
**What happened:** 175.45.176.3 → 149.171.126.10  
**Why flagged:** MAX_TTL = 9.165, 319.9x benign-typical error; MIN_TTL = 9.153, 43.7x benign-typical error  
**Behaviour hypothesis:** consistent with a stealthy probe or misconfigured host sending packets with abnormally low TTLs.  
**Recommended action:** Investigate the source host for misconfiguration or compromise; block traffic from 175.45.176.3 if no legitimate service is expected.

| feature | value (z) | error × benign | IG attribution |
|--------:|----------:|---------------:|---------------:|
| `MAX_TTL` | 9.165 | 319.9× | +97.728 |
| `MIN_TTL` | 9.153 | 43.7× | +91.465 |
| `LONGEST_FLOW_PKT` | 1.256 | 0.2× | -3.957 |
| `NUM_PKTS_UP_TO_128_BYTES` | -0.547 | 0.3× | -2.713 |
| `MIN_IP_PKT_LEN` | -1.61 | 0.2× | +2.581 |

---

## 🚨 15 · 🟠 **HIGH** · `Exploits`

> **175.45.176.3 → 149.171.126.13** · score **209.7** vs threshold **126.7**

**Severity:** high — “Unusual TTL, protocol anomaly 🚨”  
**What happened:** 175.45.176.3 → 149.171.126.13  
**Why flagged:** MIN_TTL = 9.153, 42.2x benign‑typical error; MAX_TTL = 9.165, 319.4x benign‑typical error; L7_PROTO = 10.0, 46.2x benign‑typical error.  
**Behaviour hypothesis:** consistent with a stealthy, low‑TTL beaconing attempt.  
**Recommended action:** block the source IP and investigate outbound traffic for similar TTL patterns.

| feature | value (z) | error × benign | IG attribution |
|--------:|----------:|---------------:|---------------:|
| `MIN_TTL` | 9.153 | 42.2× | +88.289 |
| `MAX_TTL` | 9.165 | 319.4× | +85.413 |
| `L7_PROTO` | 10.0 | 46.2× | +19.324 |
| `MIN_IP_PKT_LEN` | -1.61 | 0.2× | +1.099 |
| `NUM_PKTS_UP_TO_128_BYTES` | -0.495 | 0.0× | -0.489 |

---

## 🚨 16 · 🟠 **HIGH** · `Benign`

> **59.166.0.4 → 149.171.126.7** · score **500.7** vs threshold **126.7**

**Severity:** high — Unusual traffic spike detected 🚨  
**What happened:** 59.166.0.4 → 149.171.126.7  
**Why flagged:** OUT_PKTS = 10.0, 5.3x benign-typical error; NUM_PKTS_512_TO_1024_BYTES = 10.0, 7.5x benign-typical error; SRC_TO_DST_IAT_MAX = 8.989, 18.3x benign-typical error  
**Behaviour hypothesis:** consistent with a burst of small‑packet reconnaissance activity.  
**Recommended action:** isolate 59.166.0.4 and perform packet capture for further analysis.

| feature | value (z) | error × benign | IG attribution |
|--------:|----------:|---------------:|---------------:|
| `OUT_PKTS` | 10.0 | 5.3× | +50.513 |
| `NUM_PKTS_512_TO_1024_BYTES` | 10.0 | 7.5× | +50.254 |
| `SRC_TO_DST_IAT_MAX` | 8.989 | 18.3× | +50.132 |
| `RETRANSMITTED_OUT_BYTES` | 10.0 | 3.9× | +49.368 |
| `NUM_PKTS_1024_TO_1514_BYTES` | 10.0 | 3.9× | +49.042 |

---

## 🚨 17 · 🟠 **HIGH** · `Benign`

> **59.166.0.1 → 149.171.126.2** · score **281.3** vs threshold **126.7**

**Severity:** high — Suspicious traffic detected 🚨  
**What happened:** 59.166.0.1 → 149.171.126.2  
**Why flagged:** SRC_TO_DST_IAT_MAX = 9.348, 18.6x benign-typical error; DST_TO_SRC_IAT_MAX = 10.0, 13.3x benign-typical error; NUM_PKTS_512_TO_1024_BYTES = 9.306, 6.0x benign-typical error  
**Behaviour hypothesis:** consistent with a potential data exfiltration or command‑and‑control channel.  
**Recommended action:** Immediately isolate the source host and conduct a packet capture for deeper forensic analysis.

| feature | value (z) | error × benign | IG attribution |
|--------:|----------:|---------------:|---------------:|
| `SRC_TO_DST_IAT_MAX` | 9.348 | 18.6× | +49.243 |
| `DST_TO_SRC_IAT_MAX` | 10.0 | 13.3× | +42.945 |
| `NUM_PKTS_512_TO_1024_BYTES` | 9.306 | 6.0× | +40.738 |
| `DURATION_OUT` | 8.325 | 13.2× | +24.562 |
| `RETRANSMITTED_OUT_BYTES` | 7.057 | 1.2× | +21.367 |

---

## 🚨 18 · 🟠 **HIGH** · `Benign`

> **59.166.0.1 → 149.171.126.3** · score **388.1** vs threshold **126.7**

**Severity:** high — High risk activity detected 🚨  
**What happened:** 59.166.0.1 → 149.171.126.3  
**Why flagged:** SERVER_TCP_FLAGS = 10.0, 91.3x benign-typical error; DURATION_IN = 10.0, 95.8x benign-typical error; DURATION_OUT = 10.0, 21.9x benign-typical error  
**Behaviour hypothesis:** consistent with a prolonged, flag‑heavy connection that deviates markedly from normal traffic patterns.  
**Recommended action:** Immediately isolate 59.166.0.1 and investigate the session for potential data exfiltration or command‑and‑control activity.

| feature | value (z) | error × benign | IG attribution |
|--------:|----------:|---------------:|---------------:|
| `SERVER_TCP_FLAGS` | 10.0 | 91.3× | +60.704 |
| `DURATION_IN` | 10.0 | 95.8× | +51.234 |
| `SRC_TO_DST_IAT_MAX` | 10.0 | 19.8× | +43.519 |
| `DURATION_OUT` | 10.0 | 21.9× | +38.742 |
| `DST_TO_SRC_IAT_MAX` | 10.0 | 12.5× | +33.436 |

---

## 🚨 19 · 🟠 **HIGH** · `Benign`

> **59.166.0.7 → 149.171.126.9** · score **165.8** vs threshold **126.7**

**Severity:** high — “Unusual traffic spike detected 🚨”  
**What happened:** 59.166.0.7 → 149.171.126.9  
**Why flagged:** DURATION_OUT = 10.0, 22x benign‑typical error; SERVER_TCP_FLAGS = 6.234, 30x benign‑typical error; DURATION_IN = 6.241, 30.5x benign‑typical error  
**Behaviour hypothesis:** consistent with a potential data exfiltration attempt or malicious command‑and‑control session.  
**Recommended action:** isolate the destination host and perform a packet capture for deeper forensic analysis.

| feature | value (z) | error × benign | IG attribution |
|--------:|----------:|---------------:|---------------:|
| `DURATION_OUT` | 10.0 | 22.0× | +46.724 |
| `SERVER_TCP_FLAGS` | 6.234 | 30.0× | +22.228 |
| `NUM_PKTS_1024_TO_1514_BYTES` | 6.905 | 1.3× | +21.119 |
| `RETRANSMITTED_OUT_BYTES` | 7.036 | 1.0× | +19.730 |
| `DURATION_IN` | 6.241 | 30.5× | +18.159 |

---

## 🚨 20 · 🟠 **HIGH** · `Benign`

> **59.166.0.4 → 149.171.126.7** · score **460.2** vs threshold **126.7**

**Severity:** high — Unusual outbound traffic 🚨  
**What happened:** 59.166.0.4 → 149.171.126.7  
**Why flagged:** NUM_PKTS_512_TO_1024_BYTES = 10.0, 7.5x benign-typical error; OUT_BYTES = 9.321, 14.1x benign-typical error  
**Behaviour hypothesis:** consistent with a data exfiltration attempt or compromised host communicating with an external server.  
**Recommended action:** isolate host 59.166.0.4, capture traffic for forensic analysis, and block outbound to 149.171.126.7 until investigation completes.

| feature | value (z) | error × benign | IG attribution |
|--------:|----------:|---------------:|---------------:|
| `NUM_PKTS_512_TO_1024_BYTES` | 10.0 | 7.5× | +47.963 |
| `RETRANSMITTED_OUT_BYTES` | 10.0 | 3.9× | +46.117 |
| `NUM_PKTS_1024_TO_1514_BYTES` | 10.0 | 3.9× | +44.943 |
| `OUT_PKTS` | 10.0 | 5.4× | +41.665 |
| `OUT_BYTES` | 9.321 | 14.1× | +34.367 |

---

## 🚨 21 · 🟠 **HIGH** · `Benign`

> **59.166.0.8 → 149.171.126.1** · score **278.3** vs threshold **126.7**

**Severity:** high — Suspicious traffic spike 🚨  
**What happened:** 59.166.0.8 → 149.171.126.1  
**Why flagged:** SRC_TO_DST_IAT_MAX = 10.0, 22.0x benign-typical error; NUM_PKTS_512_TO_1024_BYTES = 9.306, 6.0x benign-typical error  
**Behaviour hypothesis:** consistent with a potential data exfiltration attempt.  
**Recommended action:** isolate the source host and block outbound traffic to 149.171.126.1.

| feature | value (z) | error × benign | IG attribution |
|--------:|----------:|---------------:|---------------:|
| `SRC_TO_DST_IAT_MAX` | 10.0 | 22.0× | +57.360 |
| `DST_TO_SRC_IAT_MAX` | 10.0 | 13.3× | +42.227 |
| `NUM_PKTS_512_TO_1024_BYTES` | 9.306 | 6.0× | +39.575 |
| `RETRANSMITTED_OUT_BYTES` | 7.057 | 1.2× | +21.702 |
| `OUT_PKTS` | 7.236 | 2.0× | +19.112 |

---

## 🚨 22 · 🟠 **HIGH** · `Benign`

> **59.166.0.9 → 149.171.126.2** · score **387.0** vs threshold **126.7**

**Severity:** high — suspicious traffic spike 🚨  
**What happened:** 59.166.0.9 → 149.171.126.2  
**Why flagged:** SRC_TO_DST_IAT_MAX = 10.0, 21.3x benign-typical error; DURATION_OUT = 10.0, 22.0x error; SERVER_TCP_FLAGS = 7.995, 54.4x error  
**Behaviour hypothesis:** consistent with a potential data exfiltration attempt or command‑and‑control beacon.  
**Recommended action:** isolate the source host and perform a packet capture for deeper forensic analysis.

| feature | value (z) | error × benign | IG attribution |
|--------:|----------:|---------------:|---------------:|
| `SRC_TO_DST_IAT_MAX` | 10.0 | 21.3× | +53.739 |
| `NUM_PKTS_512_TO_1024_BYTES` | 9.306 | 6.5× | +45.416 |
| `DURATION_OUT` | 10.0 | 22.0× | +41.777 |
| `DST_TO_SRC_IAT_MAX` | 10.0 | 13.0× | +40.000 |
| `SERVER_TCP_FLAGS` | 7.995 | 54.4× | +36.601 |

---

## 🚨 23 · 🟠 **HIGH** · `Benign`

> **59.166.0.1 → 149.171.126.0** · score **268.3** vs threshold **126.7**

**Severity:** high — suspicious traffic spike 🚨  
**What happened:** 59.166.0.1 → 149.171.126.0  
**Why flagged:** SRC_TO_DST_IAT_MAX = 9.947, 21.9x benign-typical error; NUM_PKTS_512_TO_1024_BYTES = 9.306, 6.0x error; DST_TO_SRC_IAT_MAX = 10.0, 13.4x error  
**Behaviour hypothesis:** consistent with a bursty, bidirectional data exfiltration attempt.  
**Recommended action:** isolate destination host, capture traffic for forensic analysis.

| feature | value (z) | error × benign | IG attribution |
|--------:|----------:|---------------:|---------------:|
| `SRC_TO_DST_IAT_MAX` | 9.947 | 21.9× | +57.662 |
| `DST_TO_SRC_IAT_MAX` | 10.0 | 13.4× | +42.499 |
| `NUM_PKTS_512_TO_1024_BYTES` | 9.306 | 6.0× | +41.858 |
| `RETRANSMITTED_OUT_BYTES` | 7.057 | 1.2× | +21.398 |
| `OUT_PKTS` | 7.236 | 1.9× | +20.823 |

---

## 🚨 24 · 🟠 **HIGH** · `Benign`

> **10.40.182.1 → 224.0.0.5** · score **398.6** vs threshold **126.7**

**Severity:** high — *Massive multicast anomaly detected 🚨*  
**What happened:** 10.40.182.1 → 224.0.0.5  
**Why flagged:** SRC_TO_DST_IAT_AVG = 10.0, 435.2x benign-typical error; SERVER_TCP_FLAGS = 10.0, 101.9x error; DURATION_IN = 10.0, 102.6x error  
**Behaviour hypothesis:** consistent with a potential multicast flood or misconfigured router sending excessive traffic.  
**Recommended action:** Immediately isolate the source host and inspect multicast routing tables for misconfigurations.

| feature | value (z) | error × benign | IG attribution |
|--------:|----------:|---------------:|---------------:|
| `SRC_TO_DST_IAT_AVG` | 10.0 | 435.2× | +99.034 |
| `SERVER_TCP_FLAGS` | 10.0 | 101.9× | +72.869 |
| `DURATION_IN` | 10.0 | 102.6× | +70.130 |
| `SRC_TO_DST_IAT_MAX` | 10.0 | 21.8× | +62.714 |
| `PROTOCOL` | 10.0 | 53.2× | +49.388 |

---

## 🚨 25 · 🟠 **HIGH** · `Benign`

> **59.166.0.3 → 149.171.126.7** · score **400.4** vs threshold **126.7**

**Severity:** high — “Unusual traffic spike detected 🚨”  
**What happened:** 59.166.0.3 → 149.171.126.7  
**Why flagged:** RETRANSMITTED_OUT_BYTES = 10.0, 3.8x benign-typical error; OUT_PKTS = 10.0, 5.2x benign-typical error; NUM_PKTS_512_TO_1024_BYTES = 10.0, 7.3x benign-typical error  
**Behaviour hypothesis:** consistent with a potential data exfiltration attempt or misconfigured application generating excessive retransmissions.  
**Recommended action:** Immediately isolate the source host and perform packet capture to verify payload integrity.

| feature | value (z) | error × benign | IG attribution |
|--------:|----------:|---------------:|---------------:|
| `RETRANSMITTED_OUT_BYTES` | 10.0 | 3.8× | +49.214 |
| `OUT_PKTS` | 10.0 | 5.2× | +48.158 |
| `NUM_PKTS_512_TO_1024_BYTES` | 10.0 | 7.3× | +46.444 |
| `NUM_PKTS_1024_TO_1514_BYTES` | 9.66 | 3.4× | +43.634 |
| `IN_PKTS` | 10.0 | 3.8× | +35.393 |

---

## 🚨 26 · 🟠 **HIGH** · `Benign`

> **59.166.0.9 → 149.171.126.6** · score **393.6** vs threshold **126.7**

**Severity:** high — suspicious outbound traffic 🚨  
**What happened:** 59.166.0.9 → 149.171.126.6  
**Why flagged:** OUT_PKTS = 10.0, 5.2x benign‑typical error; RETRANSMITTED_OUT_BYTES = 10.0, 3.8x error; NUM_PKTS_1024_TO_1514_BYTES = 10.0, 3.7x error.  
**Behaviour hypothesis:** consistent with a potential data exfiltration attempt.  
**Recommended action:** isolate host 59.166.0.9 and conduct packet capture for forensic analysis.

| feature | value (z) | error × benign | IG attribution |
|--------:|----------:|---------------:|---------------:|
| `OUT_PKTS` | 10.0 | 5.2× | +49.263 |
| `RETRANSMITTED_OUT_BYTES` | 10.0 | 3.8× | +48.097 |
| `NUM_PKTS_1024_TO_1514_BYTES` | 10.0 | 3.7× | +46.438 |
| `NUM_PKTS_512_TO_1024_BYTES` | 10.0 | 7.2× | +46.217 |
| `IN_PKTS` | 10.0 | 3.9× | +35.962 |

---

## 🚨 27 · 🟠 **HIGH** · `Benign`

> **59.166.0.2 → 149.171.126.9** · score **137.9** vs threshold **126.7**

**Severity:** high — Unusual traffic spike detected 🚨  
**What happened:** 59.166.0.2 → 149.171.126.9  
**Why flagged:** NUM_PKTS_512_TO_1024_BYTES = 9.306, 5.3x error; RETRANSMITTED_OUT_BYTES = 7.057, 1.2x error; OUT_PKTS = 7.236, 1.8x error  
**Behaviour hypothesis:** consistent with anomalous data exfiltration attempts.  
**Recommended action:** isolate the source host and block outbound traffic to 149.171.126.9.

| feature | value (z) | error × benign | IG attribution |
|--------:|----------:|---------------:|---------------:|
| `NUM_PKTS_512_TO_1024_BYTES` | 9.306 | 5.3× | +33.795 |
| `RETRANSMITTED_OUT_BYTES` | 7.057 | 1.2× | +22.461 |
| `OUT_PKTS` | 7.236 | 1.8× | +17.927 |
| `NUM_PKTS_1024_TO_1514_BYTES` | 6.747 | 1.0× | +15.074 |
| `IN_PKTS` | 7.063 | 1.0× | +9.212 |

---

## 🚨 28 · 🟠 **HIGH** · `Benign`

> **59.166.0.9 → 149.171.126.2** · score **211.5** vs threshold **126.7**

**Severity:** high — *Unusual traffic spike detected 🚨*  
**What happened:** 59.166.0.9 → 149.171.126.2  
**Why flagged:** DURATION_OUT = 10.0, 22.4x benign-typical error; SERVER_TCP_FLAGS = 8.353, 60.7x benign-typical error; DURATION_IN = 8.361, 62.9x benign-typical error  
**Behaviour hypothesis:** consistent with a potential data exfiltration attempt or command‑and‑control session.  
**Recommended action:** isolate the destination host and perform a packet capture for forensic analysis.

| feature | value (z) | error × benign | IG attribution |
|--------:|----------:|---------------:|---------------:|
| `DURATION_OUT` | 10.0 | 22.4× | +47.212 |
| `SERVER_TCP_FLAGS` | 8.353 | 60.7× | +42.477 |
| `DURATION_IN` | 8.361 | 62.9× | +38.461 |
| `NUM_PKTS_1024_TO_1514_BYTES` | 6.905 | 1.4× | +23.602 |
| `RETRANSMITTED_OUT_BYTES` | 7.036 | 1.0× | +18.594 |

---

## 🚨 29 · 🟠 **HIGH** · `Benign`

> **59.166.0.1 → 149.171.126.8** · score **459.0** vs threshold **126.7**

**Severity:** high — Unusual traffic spike 🚨  
**What happened:** 59.166.0.1 → 149.171.126.8  
**Why flagged:** RETRANSMITTED_OUT_BYTES = 10.0, 3.8x benign-typical error; NUM_PKTS_512_TO_1024_BYTES = 10.0, 7.6x benign-typical error  
**Behaviour hypothesis:** consistent with a potential data exfiltration attempt or misconfigured client.  
**Recommended action:** Investigate the session, capture packet trace, and isolate the source host.

| feature | value (z) | error × benign | IG attribution |
|--------:|----------:|---------------:|---------------:|
| `RETRANSMITTED_OUT_BYTES` | 10.0 | 3.8× | +50.928 |
| `NUM_PKTS_1024_TO_1514_BYTES` | 10.0 | 3.9× | +48.133 |
| `NUM_PKTS_512_TO_1024_BYTES` | 10.0 | 7.6× | +46.754 |
| `OUT_PKTS` | 10.0 | 5.4× | +46.255 |
| `IN_PKTS` | 10.0 | 4.0× | +36.024 |

---

## 🚨 30 · 🟠 **HIGH** · `Benign`

> **59.166.0.0 → 149.171.126.2** · score **132.1** vs threshold **126.7**

**Severity:** high — *Anomalous traffic spike 🚨*  
**What happened:** 59.166.0.0 → 149.171.126.2  
**Why flagged:** NUM_PKTS_512_TO_1024_BYTES = 9.306, 5.2x benign-typical error; OUT_PKTS = 7.236, 1.8x benign-typical error  
**Behaviour hypothesis:** consistent with a potential data exfiltration attempt.  
**Recommended action:** isolate destination host and perform packet capture for forensic analysis.

| feature | value (z) | error × benign | IG attribution |
|--------:|----------:|---------------:|---------------:|
| `NUM_PKTS_512_TO_1024_BYTES` | 9.306 | 5.2× | +35.680 |
| `RETRANSMITTED_OUT_BYTES` | 7.057 | 1.3× | +21.582 |
| `OUT_PKTS` | 7.236 | 1.8× | +19.216 |
| `NUM_PKTS_1024_TO_1514_BYTES` | 6.747 | 1.0× | +14.825 |
| `IN_PKTS` | 7.063 | 1.1× | +8.892 |

---

## 🕳️ 31 · 🕳️ **DETECTION GAP** · `Exploits`

> **175.45.176.0 → 149.171.126.10** · score **17.4** vs threshold **126.7** · gap **109.3**

**Detection gap:** Model missed exploit due to score 17.4, 109.3 below threshold 126.7  
**What happened:** 175.45.176.0 → 149.171.126.10  
**Why flagged:** MAX_TTL = 1.185, 6.5x benign-typical error; MIN_TTL = 1.178, 0.8x error  
**Behaviour hypothesis:** consistent with anomalous TTL manipulation in exploit traffic.  
**Recommended action:** Investigate traffic for potential exploitation and apply stricter TTL filtering.

| feature | value (z) | error × benign | IG attribution |
|--------:|----------:|---------------:|---------------:|
| `MAX_TTL` | 1.185 | 6.5× | +2.305 |
| `MIN_TTL` | 1.178 | 0.8× | +2.060 |
| `L4_DST_PORT` | -0.623 | 0.7× | -1.217 |
| `DST_TO_SRC_IAT_AVG` | 1.623 | 0.1× | +1.213 |
| `FTP_COMMAND_RET_CODE` | -0.464 | 0.0× | -1.032 |

---

## 🕳️ 32 · 🕳️ **DETECTION GAP** · `Exploits`

> **175.45.176.3 → 149.171.126.10** · score **19.6** vs threshold **126.7** · gap **107.1**

**Detection gap:** The model missed an exploit attempt because the score (19.6) fell 107.1 below the threshold (126.7). Key anomalous features—DST_TO_SRC_IAT_AVG (1.949, 0.6), MIN_TTL (1.178, 0.7), MAX_TTL (1.185, 5.8)—were not weighted heavily enough to push the score over the cutoff. The low attribution of ICMP_IPV4_TYPE and L4_DST_PORT further diluted the overall anomaly signal.

| feature | value (z) | error × benign | IG attribution |
|--------:|----------:|---------------:|---------------:|
| `DST_TO_SRC_IAT_AVG` | 1.949 | 0.6× | +2.002 |
| `MIN_TTL` | 1.178 | 0.7× | +1.848 |
| `MAX_TTL` | 1.185 | 5.8× | +1.726 |
| `ICMP_IPV4_TYPE` | -0.963 | 0.1× | -1.596 |
| `L4_DST_PORT` | -0.62 | 0.6× | -1.145 |

---

## 🕳️ 33 · 🕳️ **DETECTION GAP** · `Exploits`

> **175.45.176.3 → 149.171.126.19** · score **41.0** vs threshold **126.7** · gap **85.7**

**Detection gap:** missed due to score 41.0 far below threshold 126.7 (distance 85.7) despite high L7_PROTO anomaly (value 10.0, 33.8× error).  
**What happened:** 175.45.176.3 → 149.171.126.19  
**Why flagged:** L7_PROTO = 10.0, 33.8× benign-typical error; MIN_TTL = 1.178, 0.5× error; MAX_TTL = 1.185, 4.7× error.  
**Behaviour hypothesis:** consistent with stealthy exploitation traffic.  
**Recommended action:** investigate FTP_COMMAND_RET_CODE 1.274 for potential command injection.

| feature | value (z) | error × benign | IG attribution |
|--------:|----------:|---------------:|---------------:|
| `L7_PROTO` | 10.0 | 33.8× | +20.478 |
| `MIN_TTL` | 1.178 | 0.5× | +0.955 |
| `MAX_TTL` | 1.185 | 4.7× | +0.732 |
| `FTP_COMMAND_RET_CODE` | 1.274 | 0.0× | +0.694 |
| `PROTOCOL` | -0.471 | 0.1× | -0.459 |

---

## 🕳️ 34 · 🕳️ **DETECTION GAP** · `Reconnaissance`

> **175.45.176.3 → 149.171.126.13** · score **23.7** vs threshold **126.7** · gap **103.1**

**Detection gap:** Model missed due to low score (23.7) far below threshold (126.7) despite high MAX_TTL error_ratio (6.1).  
**What happened:** 175.45.176.3 → 149.171.126.13  
**Why flagged:** MAX_TTL = 1.185, 6.1x benign-typical error; TCP_WIN_MAX_IN = 2.252, 0.5x error.  
**Behaviour hypothesis:** consistent with subtle reconnaissance traffic.  
**Recommended action:** Review and adjust threshold for MAX_TTL, add rule to flag high TCP window anomalies.

| feature | value (z) | error × benign | IG attribution |
|--------:|----------:|---------------:|---------------:|
| `TCP_WIN_MAX_IN` | 2.252 | 0.5× | +2.402 |
| `MIN_TTL` | 1.178 | 0.5× | +1.514 |
| `FTP_COMMAND_RET_CODE` | -0.464 | 0.0× | -1.353 |
| `L4_DST_PORT` | -0.578 | 0.4× | -1.215 |
| `MAX_TTL` | 1.185 | 6.1× | +1.070 |

---

## 🕳️ 35 · 🕳️ **DETECTION GAP** · `Generic`

> **175.45.176.3 → 149.171.126.15** · score **22.2** vs threshold **126.7** · gap **104.5**

**Detection gap:** missed due to score 22.2 < threshold 126.7 (distance 104.5)  
**What happened:** 175.45.176.3 → 149.171.126.15  
**Why flagged:** MIN_TTL = 1.178, 0.7 benign‑typical error; TCP_WIN_MAX_IN = 1.264, 0.3 benign‑typical error; MAX_TTL = 1.185, 7.6 benign‑typical error; FTP_COMMAND_RET_CODE = -0.464, 0.0 benign‑typical error; ICMP_IPV4_TYPE = 1.403, 0.7 benign‑typical error.  
**Behaviour hypothesis:** consistent with anomalous low‑TTL traffic possibly evading detection.  
**Recommended action:** review low‑TTL flows and adjust model threshold or feature weighting.

| feature | value (z) | error × benign | IG attribution |
|--------:|----------:|---------------:|---------------:|
| `MIN_TTL` | 1.178 | 0.7× | +1.928 |
| `TCP_WIN_MAX_IN` | 1.264 | 0.3× | +1.840 |
| `MAX_TTL` | 1.185 | 7.6× | +1.499 |
| `FTP_COMMAND_RET_CODE` | -0.464 | 0.0× | -1.487 |
| `ICMP_IPV4_TYPE` | 1.403 | 0.7× | +1.221 |

---

## 🕳️ 36 · 🕳️ **DETECTION GAP** · `Reconnaissance`

> **175.45.176.2 → 149.171.126.18** · score **17.9** vs threshold **126.7** · gap **108.8**

**Detection gap:** The model missed the event because the score (17.9) fell 108.8 below the threshold (126.7). Key anomalies—TCP_WIN_MAX_IN (2.814, 1.6× error) and MAX_TTL (1.185, 6.5× error)—were not weighted enough to push the score over the cutoff. The benign‑typical error ratios for MIN_TTL (0.5×) and ICMP_IPV4_TYPE (0.4×) further diluted the overall anomaly signal.

| feature | value (z) | error × benign | IG attribution |
|--------:|----------:|---------------:|---------------:|
| `TCP_WIN_MAX_IN` | 2.814 | 1.6× | +4.324 |
| `MAX_TTL` | 1.185 | 6.5× | +2.357 |
| `MIN_TTL` | 1.178 | 0.5× | +2.042 |
| `ICMP_IPV4_TYPE` | 1.403 | 0.4× | +0.900 |
| `FTP_COMMAND_RET_CODE` | -0.464 | 0.2× | -0.832 |

---

*Generated 2026-11-22 13:22 · GraphIDS Phase 4 explainability pipeline*