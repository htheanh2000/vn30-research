# Research Proposal
# Mispricing and Arbitrage Opportunities in Vietnam's VN30 Index Futures: Evidence from a Nascent Derivatives Market

> **Solo Author:** [Tên bạn], CFA, MBA
> **Target Journal:** Finance Research Letters (Q1, Elsevier) — short paper ~4,000 từ, review nhanh
> **Backup Journals:** Borsa Istanbul Review (Q2, OA), Research in International Business and Finance (Q1)
> **Timeline dự kiến:** 3-4 tháng

---

## I. INTRODUCTION — Tại sao bài này cần tồn tại?

### 1.1 Bối cảnh

Thị trường phái sinh Việt Nam ra đời ngày **10/08/2017** với sản phẩm đầu tiên và duy nhất là **hợp đồng tương lai chỉ số VN30** (VN30F) trên Sở GDCK Hà Nội (HNX). Đến nay:

| Chỉ số | Giá trị (ước ~2025-2026) |
|--------|------------------------|
| Thời gian hoạt động | ~8 năm |
| Sản phẩm | VN30F (1 tháng, 2 tháng, 1 quý, 2 quý) |
| Khối lượng GD/ngày | ~150,000-250,000 hợp đồng |
| Open Interest | ~30,000-50,000 hợp đồng |
| Multiplier | 100,000 VND/điểm index |
| Daily limit | ±7% |
| Margin | ~10-15% |

Thị trường đã tăng trưởng mạnh về thanh khoản nhưng câu hỏi cốt lõi chưa được trả lời:

> *"VN30 Futures có được định giá đúng theo lý thuyết cost-of-carry không? Nếu sai lệch, mức độ bao nhiêu? Và nhà đầu tư có thể khai thác được không sau khi trừ chi phí giao dịch?"*

### 1.2 Research Gap — Khoảng trống

| Nghiên cứu hiện có về VN30F | Câu hỏi đã trả lời | Câu hỏi CHƯA trả lời |
|------------------------------|--------------------|-----------------------|
| Nguyen et al. (2019) — Price discovery | Futures hay spot dẫn dắt? | Mispricing bao nhiêu? |
| MDPI (2021) — Impact of introduction | VN30F ảnh hưởng gì đến returns? | Cost-of-carry fair value? |
| Do et al. (2021) — ETF arbitrage | ETF E1VFVN30 có arbitrage? | Futures arbitrage? |
| Pacific-Basin (2022) — Liquidity effects | Thanh khoản thay đổi ra sao? | Arbitrage bounds? |
| Nguyen et al. (2026) — Random walk | Thị trường efficient dạng yếu? | Mispricing magnitude? |
| **Samarakoon (2025) — Global comparison** | **16 markets so sánh** | **KHÔNG có Vietnam** |

**Gap rõ ràng:** Không có nghiên cứu nào đo lường **mức độ mispricing** của VN30F bằng cost-of-carry model và đánh giá **arbitrage opportunity** sau khi tính transaction costs.

### 1.3 Research Questions

1. **RQ1:** Mức độ mispricing (basis) của VN30 Index Futures so với theoretical fair value (cost-of-carry) là bao nhiêu?
2. **RQ2:** Mispricing có vượt qua no-arbitrage bounds (sau khi tính transaction costs) không? Nếu có, tần suất và thời gian tồn tại?
3. **RQ3:** Yếu tố nào giải thích mức độ mispricing? (time-to-maturity, volatility, volume, market regime)

### 1.4 Contribution (Đóng góp)

1. **Empirical:** Nghiên cứu **đầu tiên** đo lường mispricing VN30F bằng cost-of-carry — lấp đầy gap trong literature
2. **Comparative:** So sánh mispricing VN30F với benchmark quốc tế (S&P 500 ~20-75bp per MacKinlay & Ramaswamy 1988; Nifty 50, IBOVESPA per Samarakoon 2025) → VN nằm ở đâu?
3. **Practical:** Kết quả trực tiếp hữu ích cho traders, quant funds, và regulators → actionable insights
4. **Policy:** Hàm ý cho HNX/UBCKNN về cải thiện market efficiency

---

## II. LITERATURE REVIEW — Khung lý thuyết

### 2.1 Cost-of-Carry Model — Nền tảng

Theoretical fair value của index futures:

```
F* = S × e^{(r - d) × T}

Trong đó:
F* = Fair value (giá lý thuyết)
S  = Spot index (VN30 Index)
r  = Risk-free rate (lãi suất phi rủi ro — dùng lãi suất TPCP VN hoặc interbank)
d  = Dividend yield (tỷ suất cổ tức VN30)
T  = Time to maturity (thời gian đến đáo hạn, tính theo năm)
```

**Mispricing (Basis):**

```
Mispricing = F_market - F*
           = F_market - S × e^{(r - d) × T}

Relative Mispricing (%) = (F_market - F*) / S × 100
```

### 2.2 No-Arbitrage Bounds — Vùng không arbitrage

Khi tính transaction costs, mispricing chỉ "khai thác được" khi vượt qua bounds:

```
UPPER BOUND (overpriced → cash-and-carry arbitrage):
F_market > S × e^{(r + tc_buy_stock + tc_sell_futures) × T}
→ Mua cổ phiếu + Bán futures → lock profit

LOWER BOUND (underpriced → reverse cash-and-carry):
F_market < S × e^{(r - d - tc_sell_stock - tc_buy_futures) × T}
→ Short cổ phiếu + Mua futures → lock profit
⚠️ Tại VN: short-selling RẤT KHÓ → lower bound gần như không khai thác được
```

**Transaction costs tại VN (ước tính):**

| Chi phí | Mức | Ghi chú |
|---------|-----|---------|
| Phí mua/bán cổ phiếu | ~0.15-0.25% mỗi chiều | Tùy broker |
| Phí giao dịch futures | ~3,000-5,000 VND/HĐ | ≈ 0.002-0.003% |
| Thuế bán cổ phiếu | 0.1% | Chỉ khi bán |
| Bid-ask spread (VN30F) | ~0.1-0.3 index points | Tùy thanh khoản |
| Bid-ask spread (cổ phiếu) | ~0.1-0.5% | Tùy mã |
| Market impact cost | Variable | Tùy order size |
| **Tổng ước tính 1 chiều** | **~0.4-0.8%** | **= 40-80 basis points** |

> 📝 **Insight quan trọng:** Transaction costs tại VN (~40-80bp mỗi chiều) **cao hơn nhiều** so với developed markets (S&P 500: ~5-15bp). Điều này mở rộng no-arbitrage bounds → mispricing có thể "tồn tại" lâu hơn mà không bị arbitrage away.

### 2.3 Literature Timeline

```
1983  Cornell & French ──── Bài đầu tiên: cost-of-carry cho S&P 500
  │
1988  MacKinlay & Ramaswamy ── Kinh điển: mispricing ~20-75bp, intraday
  │                              data, arbitrage violations
1991  Chung (1991) ──────── MMI futures, transactions data test
  │
1994  Yadav & Pope ──────── FTSE 100: "profit hay risk premium?"
  │
2006  Draper & Fung ─────── Cross-listed Nikkei futures
  │
2007  Białkowski & Jakubowski ── Poland (emerging): significant arb bounds
  │
2022  Chen (JFM) ────────── Nonlinear limits to arbitrage
  │
2025  Samarakoon et al. ──── 16 global markets, VAR/ARX, emerging > developed
  │                          ⚠️ KHÔNG có Vietnam
2025  Wu (AIMS) ─────────── Fractal model for futures pricing
  │
2026  BÀI CỦA BẠN ────────── VN30F mispricing, cost-of-carry
       Extends: MacKinlay (1988) + Samarakoon (2025) → Vietnam
```

### 2.4 Hypotheses

Dựa trên literature, đặc biệt phát hiện emerging markets có mispricing lớn hơn (Samarakoon 2025) và VN có transaction costs cao + không short-sell được:

> **H1:** VN30 Futures có mức mispricing trung bình **lớn hơn** các developed markets (>75bp).

> **H2:** Upper boundary violations (overpricing) **phổ biến hơn** lower boundary violations, do short-selling constraints trên thị trường cổ phiếu VN.

> **H3:** Mispricing **giảm dần theo thời gian** khi thị trường mature (so sánh 2017-2020 vs. 2021-2026).

> **H4:** Mispricing lớn hơn khi: (a) time-to-maturity ngắn, (b) volatility cao, (c) volume thấp.

---

## III. METHODOLOGY — Phương pháp

### 3.1 Data

| Dữ liệu | Nguồn | Tần suất | Giai đoạn |
|---------|-------|---------|----------|
| **VN30F prices** (near-month contract) | HNX, Vietstock, Fiintrade, hoặc Bloomberg | Daily close | 08/2017 – 03/2026 |
| **VN30 Index** | HOSE | Daily close | 08/2017 – 03/2026 |
| **Lãi suất phi rủi ro** | TPCP kỳ hạn 3M/6M/1Y (SBV, Bloomberg) | Daily/Weekly | 08/2017 – 03/2026 |
| **Dividend yield VN30** | Fiintrade, Bloomberg, tự tính từ cổ tức 30 mã | Quarterly estimate | 08/2017 – 03/2026 |
| **Volume & Open Interest** | HNX | Daily | 08/2017 – 03/2026 |

**Ước tính observations:** ~2,000 trading days (8 năm × ~250 ngày/năm)

**Roll convention:** Dùng **near-month (front-month) contract**, roll vào ngày giao dịch cuối cùng trước expiry sang contract tháng tiếp theo.

### 3.2 Tính toán Mispricing

**Step 1 — Fair Value:**
```python
import numpy as np

# Daily calculation
F_star = S * np.exp((r - d) * T)

# Mispricing (absolute)
mispricing = F_market - F_star

# Mispricing (relative, basis points)  
mispricing_bp = (F_market - F_star) / S * 10000
```

**Step 2 — No-Arbitrage Bounds:**
```python
# Upper bound (cash-and-carry)
upper = S * np.exp((r + tc_long) * T)

# Lower bound (reverse cash-and-carry)
lower = S * np.exp((r - d - tc_short) * T)

# Boundary violation
upper_violation = F_market > upper  # overpriced beyond arb bounds
lower_violation = F_market < lower  # underpriced beyond arb bounds
```

**Step 3 — Dividend Yield Estimation:**

Đây là phần **khó nhất** cho VN30. Hai cách:
- **Cách 1 (chính xác hơn):** Tính actual dividend payments từ 30 mã trong VN30, chia cho index level
- **Cách 2 (proxy):** Dùng trailing 12-month dividend yield từ Bloomberg/Fiintrade

> 📝 Khuyến nghị: Dùng **Cách 1** cho kết quả chính xác + robustness check bằng **Cách 2**.

### 3.3 Phân tích thống kê

#### A. Descriptive Statistics (cho H1)
- Mean, Median, Std Dev, Min, Max của mispricing (bp)
- Distribution: Histogram, Q-Q plot
- So sánh với benchmarks quốc tế (bảng)

#### B. Boundary Violation Analysis (cho H2)
- Tỷ lệ upper vs. lower violations
- Magnitude of violations (bp)
- Duration of violations (ngày)
- Chi-square test: upper violations > lower violations?

#### C. Time-Series Evolution (cho H3)
- Chia thành sub-periods:
  - **P1:** 2017-2019 (early/nascent)
  - **P2:** 2020-2021 (COVID crisis)
  - **P3:** 2022-2026 (maturing)
- So sánh mispricing across periods (t-test, Kruskal-Wallis)
- Rolling window mispricing (30/60/90 ngày)

#### D. Regression Analysis (cho H4)
```
|Mispricing_t| = α + β₁(TTM_t) + β₂(Volatility_t) + β₃(Volume_t) 
                + β₄(Open_Interest_t) + β₅(VN30_Return_t) + ε_t

Trong đó:
TTM          = Time-to-maturity (ngày)
Volatility   = Realized volatility (20-day rolling)
Volume       = Log trading volume VN30F
Open_Interest = Log open interest
VN30_Return  = Daily return VN30 Index
```

Robust standard errors (Newey-West HAC) vì time-series data có autocorrelation.

#### E. Robustness Checks
- Thay đổi proxy lãi suất (TPCP 3M vs. 6M vs. interbank)
- Thay đổi transaction cost estimates (low/mid/high scenarios)
- Thay đổi dividend yield estimation method
- Sub-sample analysis (COVID vs. non-COVID)
- Asymmetric mispricing analysis (positive vs. negative separately)

### 3.4 Tools

| Tool | Mục đích |
|------|---------|
| **Python** | Data processing, tính toán, visualization |
| `pandas` | Data manipulation |
| `numpy` | Numerical computation |
| `statsmodels` | Regression, HAC standard errors, time-series tests |
| `matplotlib/seaborn` | Charts |
| **Data source** | HNX (free), Fiintrade/Vietstock (VN provider), hoặc Bloomberg terminal |

---

## IV. EXPECTED RESULTS — Kết quả dự kiến

### Dự đoán (dựa trên literature + đặc thù VN)

| Hypothesis | Dự đoán | Lý do |
|-----------|---------|-------|
| **H1: Mispricing > developed markets** | **Likely YES, >100bp** | Transaction costs cao (~40-80bp/chiều), thanh khoản thấp hơn S&P 500, thiếu institutional arbitrageurs |
| **H2: Upper violations > Lower** | **Likely YES** | VN không short-sell cổ phiếu hiệu quả → reverse cash-and-carry không thực hiện được → lower bound không bị enforce |
| **H3: Mispricing giảm theo thời gian** | **Likely YES** | Thanh khoản tăng qua các năm, market mature hơn |
| **H4a: TTM ngắn → mispricing cao** | **Likely YES** | Near expiry: dividend uncertainty cao, rollover effects |
| **H4b: Vol cao → mispricing cao** | **Likely YES** | Uncertainty → wider no-arb bounds |
| **H4c: Volume thấp → mispricing cao** | **Likely YES** | Kém thanh khoản → ít arbitrageurs |

### Expected Key Figure

```
                    MISPRICING VN30F vs. GLOBAL BENCHMARKS
                    (hypothetical illustration)

Mispricing (bp)
    │
200 ┤                                          ╔═══╗
    │                                          ║VN30║  ← bạn đo cái này
150 ┤                              ╔═══╗       ║   ║
    │                              ║Nifty║      ║   ║
100 ┤                 ╔═══╗        ║   ║       ║   ║
    │                 ║IBOV║       ║   ║       ║   ║
 75 ┤    ╔═══╗        ║   ║       ║   ║       ║   ║
    │    ║FTSE║       ║   ║       ║   ║       ║   ║
 50 ┤    ║   ║        ║   ║       ║   ║       ║   ║
    │    ║   ║        ║   ║       ║   ║       ║   ║
 25 ┤╔═══╗   ║        ║   ║       ║   ║       ║   ║
    │║S&P║   ║        ║   ║       ║   ║       ║   ║
  0 ┤╚═══╩═══╩════════╩═══╩═══════╩═══╩═══════╩═══╝
    Developed         Emerging              Frontier
    Markets           Markets               Market
```

---

## V. PAPER STRUCTURE — Cấu trúc bài

Cho **Finance Research Letters** (~4,000 từ max):

```
1. Introduction                          (~800 từ)
   - Problem statement
   - Gap & contribution (3 bullet points)
   - Preview of findings

2. Literature & Hypotheses               (~600 từ)
   - Cost-of-carry model
   - Key references (MacKinlay 1988, Samarakoon 2025)
   - 4 hypotheses

3. Data & Methodology                    (~800 từ)
   - Data description + summary stats
   - Mispricing calculation
   - Arbitrage bounds
   - Regression specification

4. Results                               (~1,200 từ)
   - Descriptive: mispricing distribution
   - Boundary violations: upper vs. lower
   - Time evolution: subperiods
   - Determinants: regression
   - Robustness checks

5. Conclusion                            (~600 từ)
   - Main findings (3 bullets)
   - Comparison with global benchmarks
   - Practical & policy implications
   - Limitations & future research

References                               (~30-40 refs)
```

---

## VI. TIMELINE — Lộ trình

| Giai đoạn | Thời gian | Công việc |
|-----------|----------|----------|
| **Phase 1** | Tuần 1-2 | Thu thập & làm sạch data (VN30F, VN30 Index, lãi suất, cổ tức) |
| **Phase 2** | Tuần 3-4 | Code Python: tính mispricing, arbitrage bounds, descriptive stats |
| **Phase 3** | Tuần 5-6 | Regression analysis, robustness checks, tạo charts |
| **Phase 4** | Tuần 7-9 | Viết paper (Introduction, Literature, Methodology, Results) |
| **Phase 5** | Tuần 10-11 | Self-review, chỉnh sửa, format theo journal guidelines |
| **Phase 6** | Tuần 12 | Submit lên Finance Research Letters |
| **Review** | Tuần 13-20 | Chờ review (~2 tháng cho FRL) |
| **Revision** | Tuần 21-23 | Sửa theo reviewer comments |

**Tổng: ~3-4 tháng đến submission, ~5-6 tháng đến acceptance (nếu thuận lợi)**

---

## VII. DATA ACCESS — Lấy data ở đâu?

### Free sources

| Data | Source | Link/Cách lấy |
|------|--------|---------------|
| VN30F daily prices | **Vietstock** | finance.vietstock.vn → Phái sinh |
| VN30F daily prices | **CafeF** | cafef.vn → Phái sinh |
| VN30 Index | **HOSE** | hsx.vn → Chỉ số |
| Lãi suất TPCP | **HNX** | hnx.vn → Trái phiếu → Đường cong lãi suất |
| Lãi suất interbank | **SBV** | sbv.gov.vn |

### Paid (nếu cần quality data)

| Data | Source | Chi phí |
|------|--------|--------|
| Full historical VN30F | **Fiintrade / FiinPro** | ~2-5 triệu VND/tháng |
| Bloomberg terminal | University/broker access | Expensive nhưng chất lượng nhất |
| **vnstock** (Python package) | Open source | Free — `pip install vnstock` |

### Lưu ý quan trọng về Dividend Yield

Đây là phần **khó nhất**:
- VN30 Index **không công bố dividend yield chính thức**
- Cần tự tính từ lịch sử chia cổ tức 30 mã trong rổ VN30
- Hoặc dùng proxy từ Fiintrade/Bloomberg
- **Robustness check:** Test sensitivity với ±0.5% dividend yield → mispricing thay đổi bao nhiêu?

---

## VIII. RISK & MITIGATION — Rủi ro & Cách xử lý

| Rủi ro | Xác suất | Cách xử lý |
|--------|---------|-----------|
| Data VN30F không đủ quality | Trung bình | Cross-check 2 nguồn (Vietstock + CafeF) |
| Dividend yield khó tính chính xác | Cao | Robustness check: low/mid/high dividend scenarios |
| Reviewer hỏi "tại sao solo author?" | Thấp | CFA credential + industry experience = credible |
| Reviewer yêu cầu intraday data | Trung bình | State as limitation, offer daily data vẫn valid (nhiều bài kinh điển dùng daily) |
| Kết quả không interesting (mispricing quá nhỏ) | Thấp | Nếu nhỏ → **vẫn là finding**: "VN30F surprisingly efficient for a nascent market" |

---

## IX. KEY REFERENCES — Tham khảo chính

### Seminal papers
1. Cornell, B., & French, K. (1983). The pricing of stock index futures. *Journal of Futures Markets*, 3(1), 1-14.
2. **MacKinlay, A.C., & Ramaswamy, K. (1988). Index-futures arbitrage and the behavior of stock index futures prices. *Review of Financial Studies*, 1(2), 137-158.**
3. Yadav, P.K., & Pope, P.F. (1994). Stock index futures mispricing: profit opportunities or risk premia? *Journal of Banking & Finance*, 18(5), 921-953.

### Emerging markets
4. Białkowski, J., & Jakubowski, J. (2008). Stock index futures arbitrage in emerging markets: Polish evidence. *International Review of Financial Analysis*, 17(2), 363-381.
5. **Samarakoon, S.M.R.K., Pradhan, R.P., & Perera, D.A.M. (2025). Index futures mispricing: A global phenomenon? *Borsa Istanbul Review*, 25(6), 1234-1269.**

### Vietnam-specific
6. Nguyen, T.N., et al. (2019). Price discovery and information transmission across stock index futures. *Investment Management and Financial Innovations*, 16(4), 262-276.
7. Do, H.P., et al. (2021). Arbitrage with Exchange-traded Funds: A Case of E1VFVN30. *Economic Computation and Economic Cybernetics Studies and Research*, 55(SI7).
8. Nguyen, T.H.T., et al. (2026). Random walk and unbiasedness in emerging derivatives markets. *Risk Governance and Control*, 16(1), 58-66.

### Methodology
9. Newey, W.K., & West, K.D. (1987). A simple, positive semi-definite, heteroskedasticity and autocorrelation consistent covariance matrix. *Econometrica*, 55(3), 703-708.

---

*Proposal created: 2026-04-15*
*Author: Solo researcher with CFA + MBA + Engineering background*
