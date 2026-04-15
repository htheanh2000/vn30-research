# Research Proposal v2 (Expanded)

# What Drives Futures Mispricing in a Frontier Market? Evidence from Vietnam's VN30 Index Futures

> **Solo Author:** [Tên], CFA, MBA, Engineer
> **Target Journal (Primary):** Emerging Markets Review (Q1, Elsevier)
> **Target Journal (Backup):** Research in International Business and Finance (Q1) | Borsa Istanbul Review (Q2, OA)
> **Paper length:** ~7,000-9,000 từ
> **Timeline:** 4-6 tháng đến submission

---

## I. MOTIVATION & RESEARCH QUESTIONS

### 1.1 Bối cảnh

Thị trường phái sinh Việt Nam ra đời **10/08/2017** — một trong những thị trường phái sinh **trẻ nhất thế giới** — với sản phẩm duy nhất là hợp đồng tương lai chỉ số VN30 (VN30F) trên HNX.

| Đặc điểm VN30F | Chi tiết |
|----------------|---------|
| Ngày ra mắt | 10/08/2017 |
| Sản phẩm | VN30F: 1 tháng, 2 tháng, 1 quý, 2 quý |
| Multiplier | 100,000 VND/điểm index |
| Daily limit | ±7% |
| Initial margin | ~10-15% |
| KL GD/ngày (2025-26) | ~150,000-250,000 hợp đồng |
| Open Interest | ~30,000-50,000 hợp đồng |
| Short-selling cổ phiếu cơ sở | Rất hạn chế / gần như không khả thi |

Trong 8 năm hoạt động, thị trường đã trải qua:
- **COVID-19** (2020-2021): Lockdown toàn quốc, VN30 giảm ~30% trong tháng 3/2020
- **Vụ Trịnh Văn Quyết / FLC** (2022): Thao túng giá cổ phiếu lớn nhất lịch sử TTCK VN
- **Xung đột Nga-Ukraine** (2022+): Giá nguyên liệu tăng, vốn ngoại rút
- **Fed tightening** (2022-2024): Lãi suất tăng → USD/VND áp lực → vốn ngoại rút ròng
- **US-China tensions**: VN ở vị trí chiến lược → nhạy cảm với cả hai bên
- **"Ngày ma thuật"**: Biến động bất thường vào ngày đáo hạn VN30F hàng tháng → nghi vấn thao túng settlement price

### 1.2 Research Gap

**Bài báo hiện có về VN30F:**

| # | Nghiên cứu | Năm | Câu hỏi | Method |
|---|-----------|-----|---------|--------|
| 1 | Nguyen et al. — Price discovery | 2019 | Futures hay spot dẫn dắt? | VECM, Johansen |
| 2 | MDPI — Impact of introduction | 2021 | VN30F ảnh hưởng gì đến stock returns? | Event study |
| 3 | Do et al. — ETF arbitrage | 2021 | ETF E1VFVN30 có arb opportunity? | Intraday analysis |
| 4 | Pacific-Basin — Liquidity effects | 2022 | VN30F thay đổi thanh khoản cổ phiếu? | DID |
| 5 | ResearchGate — Volatility correlation | 2023 | Tương quan vol spot vs. futures qua COVID? | GARCH |
| 6 | Nguyen et al. — Random walk | 2026 | VN30F efficient dạng yếu? | ADF, KPSS, Variance ratio |

**Bài benchmark quốc tế quan trọng:**

| # | Nghiên cứu | Năm | Đóng góp |
|---|-----------|-----|---------|
| 7 | Cornell & French | 1983 | Bài đầu tiên: cost-of-carry cho S&P 500 |
| 8 | **MacKinlay & Ramaswamy** | **1988** | Kinh điển: mispricing ~20-75bp, intraday, RFS |
| 9 | Yadav & Pope | 1994 | FTSE 100: "profit hay risk premium?" |
| 10 | Białkowski & Jakubowski | 2008 | Poland (emerging): significant arb bounds |
| 11 | **Samarakoon et al.** | **2025** | 16 global markets, VAR/ARX — **KHÔNG có Vietnam** |

**GAP:**
1. ❌ Không ai đo **mispricing VN30F** bằng cost-of-carry model
2. ❌ Không ai nghiên cứu **manipulation evidence** qua expiry-day effects trên VN30F
3. ❌ Không ai test **macro + geopolitical factors** ảnh hưởng mispricing tại VN
4. ❌ Vietnam **vắng mặt** trong bài so sánh 16 thị trường của Samarakoon (2025)

### 1.3 Research Questions

> **RQ1 (Measurement):** Mức độ mispricing (basis) của VN30F so với cost-of-carry fair value là bao nhiêu? So sánh với benchmarks quốc tế ra sao?

> **RQ2 (Arbitrage):** Mispricing có vượt no-arbitrage bounds không? Upper vs. lower violations tỷ lệ thế nào? (liên quan short-selling constraints)

> **RQ3 (Manipulation):** Có evidence cho manipulation tại ngày đáo hạn VN30F không? (expiry-day mispricing anomaly)

> **RQ4 (Drivers):** Macro shocks (lãi suất SBV, FX, foreign flows) và geopolitical panic (GPR, VIX) giải thích mispricing bao nhiêu?

### 1.4 Contributions

1. **First mispricing study** cho VN30F bằng cost-of-carry → lấp gap trong literature
2. **Manipulation evidence** qua expiry-day anomaly → hàm ý cho UBCKNN/HNX
3. **Frontier market determinants** (macro + geopolitical + manipulation) → extend Samarakoon (2025) với case study Vietnam
4. **Practical:** Actionable cho quant traders, fund managers, và regulators
5. **CFA practitioner perspective** — bridge theory-practice gap

---

## II. THEORETICAL FRAMEWORK

### 2.1 Cost-of-Carry Model

```
Fair Value:    F* = S × e^{(r - d) × T}

Mispricing:    MP_t = F_market,t - F*_t

Relative:      MP_t(%) = (F_market,t - F*_t) / S_t × 100

Basis Points:  MP_t(bp) = (F_market,t - F*_t) / S_t × 10,000
```

### 2.2 No-Arbitrage Bounds

```
Upper Bound:   UB = S × e^{(r + TC_long) × T}
Lower Bound:   LB = S × e^{(r - d - TC_short) × T}

Cash-and-carry arbitrage:     F > UB → Buy stock basket + Sell futures
Reverse cash-and-carry:       F < LB → Short stock + Buy futures
                              ⚠️ Tại VN: LB gần như không enforce được
                              (short-selling constraints)
```

**Transaction costs VN (ước tính):**

| Component | Buy side | Sell side |
|-----------|----------|-----------|
| Brokerage (stock) | 0.15-0.25% | 0.15-0.25% |
| Tax on stock sale | — | 0.10% |
| Futures commission | ~0.003% | ~0.003% |
| Bid-ask spread (stock) | 0.1-0.5% | — |
| Bid-ask spread (futures) | 0.01-0.03% | — |
| Market impact | Variable | Variable |
| **Total estimate (one-way)** | **~0.4-0.8%** | **(40-80bp)** |

### 2.3 Manipulation Hypothesis — Expiry-Day Effects

Lý thuyết: Nếu participants thao túng giá settlement VN30 Index vào ngày đáo hạn (thứ 5 tuần 3 mỗi tháng) → mispricing sẽ spike bất thường vào expiry window.

```
                Normal days          Expiry window
                ─────────            ──────────────
Mispricing:     ~X bp                ~X + Δ bp (Δ > 0?)
Volume:         normal               abnormal spike?
Volatility:     normal               abnormal spike?
Reversal:       none                 end-of-day reversal?
```

### 2.4 Geopolitical Risk & Panic Transmission

```
Global Shock                    Transmission to VN30F
────────────                    ─────────────────────
VIX spike ─────────────────────→ Foreign sell-off VN stocks
                                 → Spot drops faster than futures adjust
                                 → Mispricing widens
                                 
GPR Index ↑ ───────────────────→ Uncertainty ↑
                                 → No-arb bounds widen (risk ↑)
                                 → Mispricing persistent longer

Fed Rate Hike ─────────────────→ USD/VND pressure
                                 → Foreign capital outflow
                                 → Liquidity ↓ → Mispricing ↑
                                 
SBV Policy Change ─────────────→ Cost-of-carry inputs shift
                                 → Market slow to adjust
                                 → Temporary mispricing
```

---

## III. HYPOTHESES

### Group A — Mispricing Measurement

> **H1:** Mức mispricing trung bình VN30F **lớn hơn** developed markets (>75bp), do transaction costs cao và thiếu institutional arbitrageurs.

> **H2:** Upper boundary violations (futures overpriced) **nhiều hơn** lower violations, do short-selling constraints trên thị trường cổ phiếu VN ngăn cản reverse cash-and-carry arbitrage.

> **H3:** Mispricing **giảm dần** theo thời gian khi thị trường mature (so sánh giai đoạn 2017-2020 vs. 2021-2023 vs. 2024-2026).

### Group B — Manipulation

> **H4:** Mispricing **tăng đột biến** trong expiry window (ngày đáo hạn ± 2 ngày giao dịch) so với non-expiry days, consistent với manipulation of settlement price.

> **H5:** Abnormal volume và intraday reversal patterns xuất hiện **thường xuyên hơn** trong expiry window, hỗ trợ giả thuyết thao túng.

### Group C — Macro & Geopolitical Drivers

> **H6:** Mispricing **tăng** khi SBV thay đổi lãi suất điều hành, do cost-of-carry inputs shift nhanh hơn thị trường adjust.

> **H7:** Mispricing **tăng** khi USD/VND biến động mạnh và/hoặc khối ngoại bán ròng, do liquidity shock.

> **H8:** Mispricing **tăng** khi VIX và GPR Index tăng, do panic transmission từ global → Vietnam.

---

## IV. DATA & METHODOLOGY

### 4.1 Data Sources

| Dữ liệu | Nguồn | Tần suất | Giai đoạn | Chi phí |
|---------|-------|---------|----------|--------|
| **VN30F prices** (near-month) | HNX / Vietstock / CafeF / vnstock | Daily | 08/2017 – 03/2026 | Free |
| **VN30 Index** | HOSE / Vietstock | Daily | 08/2017 – 03/2026 | Free |
| **Lãi suất TPCP VN** (3M, 6M, 1Y) | HNX / SBV / Bloomberg | Daily/Weekly | 08/2017 – 03/2026 | Free |
| **Dividend yield VN30** | Fiintrade / tự tính từ 30 mã | Quarterly | 08/2017 – 03/2026 | Free/Paid |
| **VN30F Volume & OI** | HNX | Daily | 08/2017 – 03/2026 | Free |
| **USD/VND exchange rate** | SBV / Bloomberg | Daily | 08/2017 – 03/2026 | Free |
| **Foreign net buy/sell** | HOSE | Daily | 08/2017 – 03/2026 | Free |
| **SBV policy rate changes** | SBV announcements | Event dates | 08/2017 – 03/2026 | Free |
| **Fed Funds Rate decisions** | FRED / Fed website | Event dates | 08/2017 – 03/2026 | Free |
| **VIX** (CBOE) | Yahoo Finance / FRED | Daily | 08/2017 – 03/2026 | Free |
| **GPR Index** (Geopolitical Risk) | matteoiacoviello.com | Monthly | 08/2017 – 03/2026 | Free |
| **VN30F expiry dates** | HNX rules | Monthly | 08/2017 – 03/2026 | Free |

**Estimated observations:** ~2,000 trading days

### 4.2 Variables

#### Dependent Variable
| Variable | Definition | Unit |
|----------|-----------|------|
| **\|Mispricing\|** | Absolute value of (F_market - F*) / S | Basis points |
| **Mispricing_signed** | Signed mispricing (positive = overpriced) | Basis points |
| **Boundary_Violation** | Dummy = 1 if F outside no-arb bounds | Binary |

#### Independent Variables — Microstructure (Group A)
| Variable | Proxy | Expected sign |
|----------|-------|--------------|
| TTM | Days to maturity / 365 | +/− |
| Volatility | 20-day realized volatility of VN30 | + |
| Volume | Log daily trading volume VN30F | − |
| Open_Interest | Log daily open interest | − |
| Bid_Ask | Proxy bid-ask spread (High-Low)/Close | + |

#### Independent Variables — Manipulation (Group B)
| Variable | Proxy | Expected sign |
|----------|-------|--------------|
| Expiry_Window | Dummy = 1 cho expiry day ± 2 trading days | + |
| Abnormal_Volume | Volume_t / MA20_volume > 2 | + |
| VN30_Concentration | Top-5 stock volume / total VN30 volume | + |

#### Independent Variables — Macro (Group C)
| Variable | Proxy | Expected sign |
|----------|-------|--------------|
| ΔRate_SBV | Dummy = 1 trong 5 ngày sau SBV thay đổi lãi suất | + |
| ΔUSDVND | Daily % change USD/VND | + |
| Foreign_NetSell | Foreign net sell value (negative = sell) | + |
| Fed_Decision | Dummy = 1 trong 3 ngày quanh FOMC meeting | + |
| ΔCPI_VN | Monthly CPI change (interpolated daily) | + |

#### Independent Variables — Geopolitical Panic (Group D)
| Variable | Proxy | Expected sign |
|----------|-------|--------------|
| VIX | CBOE VIX level (hoặc ΔVIX) | + |
| GPR | Geopolitical Risk Index (monthly) | + |
| COVID_Wave | Dummy cho mỗi COVID wave VN (03/2020, 07-09/2021) | + |
| RUS_UKR | Dummy từ 24/02/2022 (6 tháng) | + |

### 4.3 Econometric Models

#### Model 1 — Baseline (Microstructure only)
```
|Mispricing_t| = α + β₁TTM + β₂Vol + β₃lnVol + β₄lnOI + ε_t
```

#### Model 2 — Add Manipulation
```
|Mispricing_t| = Model 1 + γ₁Expiry + γ₂AbnVol + γ₃Concentration + ε_t
```

#### Model 3 — Add Macro
```
|Mispricing_t| = Model 2 + δ₁ΔRate + δ₂ΔFXUSDVND + δ₃ForeignNet 
                          + δ₄Fed + ε_t
```

#### Model 4 — Full Model (Add Geopolitical)
```
|Mispricing_t| = Model 3 + λ₁VIX + λ₂GPR + λ₃COVID + λ₄RUS_UKR + ε_t
```

**Estimation:** OLS with **Newey-West HAC** standard errors (correct for autocorrelation & heteroskedasticity in time-series)

**Nested model comparison:** F-test hoặc likelihood ratio test để xem mỗi group (manipulation, macro, geo) có thêm explanatory power không.

#### Model 5 — Boundary Violation (Logistic)
```
P(Violation_t = 1) = Logit(α + β₁TTM + β₂Vol + γ₁Expiry + δ₁ΔRate 
                           + λ₁VIX + ...)
```
→ Xác suất mispricing vượt no-arb bounds phụ thuộc vào factors nào?

### 4.4 Subperiod Analysis

| Period | Giai đoạn | Đặc điểm |
|--------|----------|----------|
| **P1: Nascent** | 08/2017 – 12/2019 | Thị trường mới, thanh khoản thấp |
| **P2: COVID** | 01/2020 – 12/2021 | Pandemic, lockdown, extreme volatility |
| **P3: Crisis** | 01/2022 – 12/2023 | FLC scandal, Fed hike, Nga-Ukraine, vốn ngoại rút |
| **P4: Maturing** | 01/2024 – 03/2026 | Ổn định hơn, chờ nâng hạng FTSE/MSCI |

→ So sánh mispricing magnitude & drivers across periods

### 4.5 Robustness Checks

| Check | Mục đích |
|-------|---------|
| Alternative risk-free rate (TPCP 3M vs. 6M vs. interbank) | Sensitivity to r |
| Alternative dividend yield (±0.5%) | Sensitivity to d |
| Transaction cost scenarios (low/mid/high: 30/50/80 bp) | Sensitivity to arb bounds |
| Winsorize mispricing at 1%/99% | Outlier robustness |
| GARCH-based volatility thay cho realized vol | Alternative vol measure |
| Quantile regression (10th, 50th, 90th percentiles) | Tail behavior |
| 2-month contract thay cho near-month | Alternative contract |

---

## V. EXPECTED PAPER STRUCTURE

```
1. Introduction                                    (~1,200 từ)
   - VN derivatives market context
   - Gap: no mispricing study + no manipulation + no macro/geo
   - 3 contributions
   - Preview findings

2. Literature Review                               (~1,500 từ)
   2.1 Cost-of-carry & arbitrage (Cornell 1983, MacKinlay 1988)
   2.2 Emerging/frontier market mispricing (Samarakoon 2025)
   2.3 Manipulation & expiry-day effects
   2.4 Geopolitical risk & financial markets (GPR literature)
   2.5 Vietnam's derivatives market (6 existing papers)
   2.6 Hypotheses development (H1-H8)

3. Data & Methodology                             (~1,500 từ)
   3.1 Data description & summary statistics
   3.2 Mispricing calculation & arb bounds
   3.3 Variable definitions
   3.4 Econometric specifications (Models 1-5)

4. Results                                         (~2,500 từ)
   4.1 Mispricing descriptive (magnitude, distribution, evolution)
   4.2 Boundary violations (upper vs. lower, asymmetry)
   4.3 Expiry-day anomaly (manipulation evidence)
   4.4 Regression results (Models 1→4, nested comparison)
   4.5 Logistic model (boundary violation probability)
   4.6 Subperiod analysis
   4.7 Robustness checks

5. Discussion                                      (~1,000 từ)
   5.1 Comparison with global benchmarks
   5.2 Implications for market efficiency theory
   5.3 Policy implications for UBCKNN/HNX
   5.4 Practical implications for traders

6. Conclusion                                      (~800 từ)
   - Main findings
   - Limitations
   - Future research directions

References                                         (~50-60 refs)
Appendix                                           Variable definitions, 
                                                   additional robustness
```

---

## VI. TIMELINE

| Phase | Tuần | Công việc |
|-------|------|----------|
| **1. Data Collection** | 1-3 | Thu thập VN30F, VN30, rates, FX, GPR, VIX, foreign flows. Làm sạch, merge datasets |
| **2. Mispricing Calculation** | 3-4 | Code Python: fair value, mispricing, arb bounds. Descriptive stats & charts |
| **3. Manipulation Analysis** | 5-6 | Expiry-day effects, abnormal volume, t-tests |
| **4. Regression Models** | 6-8 | Models 1→5, nested comparison, subperiod analysis |
| **5. Robustness** | 8-9 | All robustness checks, sensitivity analysis |
| **6. Writing** | 9-14 | Draft paper, tables, figures |
| **7. Self-Review** | 14-16 | Polish, proofread, format theo journal |
| **8. Submit** | 16-17 | Submit lên Emerging Markets Review |
| **9. Review Period** | 17-28 | Chờ reviewer (~2-3 tháng) |
| **10. Revision** | 28-32 | Revise & Resubmit |

**Tổng: ~4-5 tháng đến submission, ~7-8 tháng đến acceptance (optimistic)**

---

## VII. KEY REFERENCES

### Seminal: Cost-of-Carry & Mispricing
1. Cornell, B., & French, K. (1983). Pricing of stock index futures. *JFM*, 3(1), 1-14.
2. **MacKinlay, A.C., & Ramaswamy, K. (1988). Index-futures arbitrage. *RFS*, 1(2), 137-158.**
3. Yadav, P.K., & Pope, P.F. (1994). Stock index futures mispricing. *JBF*, 18(5), 921-953.
4. Białkowski, J., & Jakubowski, J. (2008). Stock index futures arbitrage in emerging markets. *IRFA*, 17(2), 363-381.
5. **Samarakoon, S.M.R.K., et al. (2025). Index futures mispricing: A global phenomenon? *BIR*, 25(6), 1234-1269.**
6. Chen, H., et al. (2022). Nonlinear limits to arbitrage. *JFM*, 42(6).

### Manipulation & Expiry Effects
7. Stoll, H., & Whaley, R. (1987). Program trading and expiration-day effects. *FAJ*, 43(2), 16-28.
8. Ni, S.X., Pearson, N.D., & Poteshman, A.M. (2005). Stock price clustering on option expiration dates. *JFE*, 78(1), 49-87.

### Geopolitical Risk
9. **Caldara, D., & Iacoviello, M. (2022). Measuring geopolitical risk. *AER*, 112(4), 1194-1225.**
10. Baker, S.R., Bloom, N., & Davis, S.J. (2016). Measuring economic policy uncertainty. *QJE*, 131(4), 1593-1636.

### Vietnam Derivatives Market
11. Nguyen, T.N., et al. (2019). Price discovery VN30 futures. *IMFI*, 16(4), 262-276.
12. Do, H.P., et al. (2021). ETF arbitrage E1VFVN30. *ECECSR*.
13. Nguyen, T.H.T., et al. (2026). Random walk in VN30 futures. *RGCFMI*, 16(1), 58-66.

### Methodology
14. Newey, W.K., & West, K.D. (1987). Heteroskedasticity and autocorrelation consistent covariance matrix. *Econometrica*, 55(3), 703-708.

---

*Proposal v2 — Created: 2026-04-15*
*Solo research project — CFA + MBA + Engineering background*
