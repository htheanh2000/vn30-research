# Cấu trúc Bài báo Khoa học aim Q1 — Hướng dẫn Chi tiết

> Dựa trên chuẩn mực của Emerging Markets Review, Research in International Business and Finance, Journal of Futures Markets, và các Q1 finance journals.

---

## TỔNG QUAN CẤU TRÚC

```
┌─────────────────────────────────────────────────────────────┐
│  TITLE                                                      │
│  ABSTRACT (150-250 từ)                                      │
│  KEYWORDS (4-6 từ)                                          │
│  JEL CLASSIFICATION (2-4 codes)                             │
├─────────────────────────────────────────────────────────────┤
│  1. INTRODUCTION                              ~1,200-1,500 từ│
│  2. LITERATURE REVIEW & HYPOTHESES            ~1,500-2,000 từ│
│  3. DATA & METHODOLOGY                        ~1,500-2,000 từ│
│  4. RESULTS                                   ~2,000-2,500 từ│
│  5. DISCUSSION                                ~800-1,200 từ  │
│  6. CONCLUSION                                ~600-800 từ    │
├─────────────────────────────────────────────────────────────┤
│  REFERENCES                                   ~50-70 refs    │
│  APPENDIX (nếu cần)                                         │
└─────────────────────────────────────────────────────────────┘

Tổng: ~7,000-10,000 từ (không tính references & appendix)
```

---

## TITLE — Tiêu đề

### Nguyên tắc
- **Ngắn gọn:** 10-15 từ là lý tưởng, tối đa 20 từ
- **Chứa:** What (chủ đề) + Where (bối cảnh) + đôi khi How (method đặc biệt)
- **KHÔNG dùng:** viết tắt, dấu chấm hỏi (trừ khi cố tình provocative), jargon quá hẹp

### Công thức phổ biến

```
Format 1: [Chủ đề chính]: Evidence from [Bối cảnh]
→ "Futures Mispricing and Market Manipulation: Evidence from Vietnam's VN30 Index"

Format 2: [Câu hỏi/Khẳng định]: [Phương pháp/Góc nhìn]
→ "What Drives Futures Mispricing in a Frontier Market? A Cost-of-Carry Analysis"

Format 3: [Hiện tượng], [Yếu tố], and [Outcome] in [Context]
→ "Manipulation, Macro Shocks, and Geopolitical Panic: Unpacking Futures Mispricing in Vietnam"

Format 4: The [relationship] between [X] and [Y]: [context]
→ "The Role of Geopolitical Risk in Index Futures Mispricing: Evidence from Vietnam"
```

### Ví dụ top papers (đã publish)
- "Index futures mispricing: A global phenomenon?" — Samarakoon (2025, BIR)
- "Index-Futures Arbitrage and the Behavior of Stock Index Futures Prices" — MacKinlay (1988, RFS)
- "Stock index futures arbitrage in emerging markets: Polish evidence" — Białkowski (2008, IRFA)

---

## ABSTRACT — Tóm tắt (150-250 từ)

### Cấu trúc bắt buộc — 5 câu/phần

```
Câu 1: BỐI CẢNH + VẤN ĐỀ
   "This study investigates [what] in [context], where [why it matters]."

Câu 2-3: PHƯƠNG PHÁP
   "Using [data description: N obs, period], we employ [method] to examine [what]."

Câu 3-4: KẾT QUẢ CHÍNH (2-3 findings cụ thể, CÓ SỐ)
   "We find that [finding 1, with number]. Furthermore, [finding 2]. 
    Notably, [finding 3 — surprising/important]."

Câu 5: HÀM Ý
   "These findings have important implications for [who: traders, regulators, policymakers]."
```

### Ví dụ draft cho bài VN30

> This study investigates the mispricing dynamics of VN30 Index Futures in Vietnam — one of the world's youngest derivatives markets — and the roles of market manipulation, macroeconomic shocks, and geopolitical risk in driving pricing inefficiencies. Using daily data spanning August 2017 to March 2026 (~2,000 observations), we measure mispricing relative to the cost-of-carry fair value and analyze arbitrage boundary violations. Our results reveal that average mispricing is approximately [X] basis points — significantly larger than developed markets (~20-75bp) and comparable to other emerging markets. Upper boundary violations dominate ([X]% vs. [Y]%), consistent with short-selling constraints preventing reverse arbitrage. We document a significant expiry-day anomaly, where mispricing spikes by [X]bp during settlement windows, providing indirect evidence of price manipulation. Furthermore, the VIX, geopolitical risk index, and foreign net selling explain [X]% of mispricing variation beyond microstructure factors. These findings offer valuable insights for traders exploiting pricing inefficiencies, regulators addressing manipulation concerns, and policymakers aiming to improve market efficiency as Vietnam pursues FTSE/MSCI emerging market reclassification.

### Lỗi phổ biến trong Abstract
- ❌ Quá chung chung, không có số cụ thể
- ❌ Viết methodology quá chi tiết (abstract không phải methodology section)
- ❌ Không nêu finding — chỉ nói "we investigate"
- ❌ Quá dài (>300 từ) hoặc quá ngắn (<100 từ)

---

## KEYWORDS & JEL

### Keywords (4-6 từ)
Chọn từ khóa để **người khác tìm được bài bạn** trên Scopus/WoS:

```
Ví dụ: Index futures mispricing; Cost-of-carry; Arbitrage; 
       Market manipulation; Geopolitical risk; Vietnam
```

### JEL Classification
Hệ thống phân loại của Journal of Economic Literature:

| Code    | Nghĩa                               | Khi nào dùng                                     |
| ------- | ----------------------------------- | ------------------------------------------------ |
| **G13** | Contingent Pricing; Futures Pricing | Bài về futures pricing → BẮT BUỘC                |
| **G14** | Information and Market Efficiency   | Bài về mispricing, efficiency                    |
| **G15** | International Financial Markets     | Bài có yếu tố cross-country hoặc emerging market |
| **G18** | Government Policy and Regulation    | Bài có policy implications (manipulation)        |
| **C32** | Time-Series Models                  | Bài dùng time-series econometrics                |
| **F37** | International Finance Forecasting   | Bài có yếu tố global risk transmission           |

Chọn **2-4 codes**, đặt code quan trọng nhất lên đầu.

---

## 1. INTRODUCTION (~1,200-1,500 từ)

### Cấu trúc Introduction — "Phễu ngược" (Inverted Funnel)

```
Đoạn 1: HOOK + BỐI CẢNH RỘNG                    (~200 từ)
    "Tại sao chủ đề này quan trọng cho thế giới?"
    
    → Mở đầu bằng fact/statistic gây ấn tượng
    → Bối cảnh lớn: emerging derivatives markets đang phát triển
    → Tại sao futures pricing matters cho market efficiency
    
Đoạn 2: THU HẸP VÀO VẤN ĐỀ CỤ THỂ               (~200 từ)
    "Vấn đề cụ thể chưa được giải quyết là gì?"
    
    → Vietnam's VN30F: đặc thù (trẻ, thiếu short-selling, manipulation concerns)
    → Bridge từ global context → Vietnam specifically
    
Đoạn 3: RESEARCH GAP                              (~300 từ)
    "Các nghiên cứu trước đã làm gì? Và thiếu gì?"
    
    → Tóm tắt 6 papers VN30F (1-2 câu mỗi bài)
    → Tóm tắt global benchmarks (MacKinlay 1988, Samarakoon 2025)
    → CHỈ RÕ gap: "However, no study has examined..."
    → Gap phải DẪN THẲNG đến RQ của bạn
    
Đoạn 4: MỤC TIÊU + RESEARCH QUESTIONS             (~200 từ)
    "Bài này làm gì để lấp gap?"
    
    → "This study aims to..."
    → List 3-4 RQs rõ ràng
    → Kết nối RQs với gap vừa nêu
    
Đoạn 5: CONTRIBUTIONS                             (~300 từ)
    "Bài này đóng góp gì mới?"
    
    → 3-4 bullet points, mỗi cái 2-3 câu
    → Contribution 1: Empirical (first study for VN)
    → Contribution 2: Methodological (manipulation evidence)
    → Contribution 3: Theoretical (extend framework to frontier market)
    → Contribution 4: Practical (implications for traders/regulators)
    
Đoạn 6: ROADMAP                                   (~50 từ)
    "The remainder of this paper is organized as follows..."
    
    → 1-2 câu liệt kê structure: Section 2 reviews..., 
      Section 3 describes..., Section 4 presents..., 
      Section 5 discusses..., Section 6 concludes.
```

### Mẹo cho Introduction Q1

1. **Câu mở đầu phải "bắt" reviewer** — dùng số liệu ấn tượng hoặc fact surprising
   - ✅ "Vietnam's VN30 futures market, launched in August 2017, has grown from zero to over 200,000 contracts traded daily — yet its pricing efficiency remains virtually unstudied."
   - ❌ "This paper studies futures mispricing in Vietnam."

2. **Gap phải tự nhiên** — reader đọc xong gap phải nghĩ "đúng, cần nghiên cứu cái này"

3. **Contributions phải cụ thể** — không nói "we contribute to the literature" mà nói "we provide the first cost-of-carry analysis of VN30 Index Futures, extending MacKinlay and Ramaswamy (1988) to a frontier derivatives market"

4. **Không review literature quá sâu** ở Introduction — chỉ cite đủ để establish gap. Chi tiết để Section 2.

---

## 2. LITERATURE REVIEW & HYPOTHESES (~1,500-2,000 từ)

### Cấu trúc

```
2.1 THEORETICAL FOUNDATION                         (~400 từ)
    → Cost-of-carry model: origin, formula, assumptions
    → No-arbitrage argument: tại sao mispricing "shouldn't" exist
    → Limits to arbitrage: tại sao nó VẪN tồn tại 
      (transaction costs, short-selling constraints, risk)

2.2 MISPRICING IN DEVELOPED MARKETS                 (~300 từ)
    → Cornell & French (1983): first study
    → MacKinlay & Ramaswamy (1988): benchmark 20-75bp
    → Yadav & Pope (1994): profit vs. risk premium debate
    → Key pattern: mispricing decreases as markets mature

2.3 MISPRICING IN EMERGING/FRONTIER MARKETS         (~300 từ)
    → Białkowski & Jakubowski (2008): Poland
    → Samarakoon et al. (2025): 16 markets, emerging > developed
    → Specific challenges: higher TC, lower liquidity, 
      short-selling constraints
    → Vietnam context: where does it fit?

2.4 MANIPULATION & EXPIRY-DAY EFFECTS               (~250 từ)
    → Stoll & Whaley (1987): expiry-day effects
    → Literature on settlement price manipulation
    → Vietnam-specific: "ngày ma thuật," FLC scandal

2.5 GEOPOLITICAL RISK & FINANCIAL MARKETS            (~250 từ)
    → Caldara & Iacoviello (2022): GPR Index — AER
    → VIX as fear gauge
    → Transmission to emerging markets
    → Vietnam's geopolitical position (US-China, Biển Đông)

2.6 VIETNAM'S DERIVATIVES MARKET                    (~200 từ)
    → 6 existing papers (brief summary each)
    → What they covered vs. what's missing

2.7 HYPOTHESES DEVELOPMENT                         (~300 từ)
    → H1-H8, mỗi hypothesis 2-3 câu justify
    → Logic: literature → gap → prediction → hypothesis
```

### Cách viết Hypothesis

```
FORMAT CHUẨN:

[Logic từ literature, 2-3 câu]
→ [Dẫn đến prediction]
→ [Hypothesis statement, in italics hoặc bold]

VÍ DỤ:

"MacKinlay and Ramaswamy (1988) document average mispricing of 
20-75 basis points for S&P 500 futures. Samarakoon et al. (2025) 
show that emerging markets exhibit significantly larger mispricing 
due to higher transaction costs and lower arbitrageur participation. 
Given that Vietnam's derivatives market is among the youngest 
globally, with transaction costs estimated at 40-80bp per leg and 
severe short-selling constraints, we expect mispricing to be 
substantially larger than in developed markets. Therefore:

**H1:** The average absolute mispricing of VN30 Index Futures 
exceeds that of developed market benchmarks (>75 basis points)."
```

### Lỗi phổ biến trong Literature Review
- ❌ **Liệt kê** papers như shopping list ("A studied X. B studied Y. C studied Z.")
- ✅ **Synthesize** — nhóm theo theme, chỉ ra patterns, conflicts, gaps
- ❌ Review quá rộng (không liên quan đến bài bạn)
- ✅ Mỗi paragraph phải **serve a purpose** — build toward your hypothesis
- ❌ Hypothesis không có justification từ literature
- ✅ Logic chain: Literature finding → Your context → Prediction → H

---

## 3. DATA & METHODOLOGY (~1,500-2,000 từ)

### Cấu trúc

```
3.1 DATA DESCRIPTION                                (~500 từ)
    → Sources: HNX, HOSE, SBV, CBOE, etc.
    → Sample period: Aug 2017 – Mar 2026
    → Frequency: daily
    → Number of observations
    → Roll convention (for futures)
    → Table 1: Summary Statistics
    
    TABLE 1: SUMMARY STATISTICS
    ┌──────────────────┬──────┬────────┬───────┬──────┬──────┐
    │ Variable         │ Obs  │ Mean   │ Std   │ Min  │ Max  │
    ├──────────────────┼──────┼────────┼───────┼──────┼──────┤
    │ VN30 Index       │ 2000 │ XXX    │ XXX   │ XXX  │ XXX  │
    │ VN30F Price      │ 2000 │ XXX    │ XXX   │ XXX  │ XXX  │
    │ Risk-free Rate   │ 2000 │ XXX    │ XXX   │ XXX  │ XXX  │
    │ Dividend Yield   │ 2000 │ XXX    │ XXX   │ XXX  │ XXX  │
    │ Mispricing (bp)  │ 2000 │ XXX    │ XXX   │ XXX  │ XXX  │
    │ VIX              │ 2000 │ XXX    │ XXX   │ XXX  │ XXX  │
    │ GPR Index        │ 2000 │ XXX    │ XXX   │ XXX  │ XXX  │
    │ ...              │      │        │       │      │      │
    └──────────────────┴──────┴────────┴───────┴──────┴──────┘

3.2 MISPRICING CALCULATION                          (~400 từ)
    → Cost-of-carry formula (with all notation defined)
    → Fair value F*
    → Mispricing = F_market - F*
    → Relative mispricing (basis points)
    → No-arbitrage bounds (upper & lower)
    → Transaction cost estimation

3.3 VARIABLE DEFINITIONS                            (~300 từ)
    → Table 2: All variables, definitions, sources, expected signs
    → Grouped: Dependent → Microstructure → Manipulation 
      → Macro → Geopolitical

3.4 ECONOMETRIC SPECIFICATION                       (~400 từ)
    → Model equations (numbered)
    → Estimation method: OLS with Newey-West HAC
    → Why Newey-West: autocorrelation in time-series
    → Nested model comparison strategy
    → Logistic model for boundary violations
    → Subperiod definition

3.5 ROBUSTNESS FRAMEWORK                            (~200 từ)
    → List all robustness checks planned
    → Alternative specifications
    → Sensitivity analysis
```

### Mẹo cho Methodology Q1

1. **Reproducible** — reader phải có thể replicate từ description
2. **Justify every choice** — "We use Newey-West standard errors because..." không chỉ "We use Newey-West."
3. **Tables > Text** — Variable definitions trong bảng, không paragraph dài
4. **Equations numbered** — Eq. (1), Eq. (2)... để reference trong Results

---

## 4. RESULTS (~2,000-2,500 từ)

### Cấu trúc

```
4.1 MISPRICING DESCRIPTIVE ANALYSIS                 (~500 từ)
    → Figure 1: Time series of mispricing (bp) over full sample
    → Figure 2: Distribution (histogram) of mispricing
    → Table 3: Mispricing by subperiod (Nascent/COVID/Crisis/Maturing)
    → Comparison with global benchmarks (MacKinlay, Samarakoon)
    → H1 result: VN mispricing > developed markets? ✅/❌

4.2 ARBITRAGE BOUNDARY VIOLATIONS                   (~300 từ)
    → Table 4: Upper vs. lower violations (count, %, magnitude)
    → Duration of violations
    → H2 result: Upper > Lower? ✅/❌
    
4.3 EXPIRY-DAY ANOMALY                             (~400 từ)
    → Table 5: Mispricing on expiry window vs. non-expiry days
    → t-test or Mann-Whitney U test
    → Figure 3: Average mispricing by day-of-month (pattern around expiry)
    → H4-H5 result: manipulation evidence? ✅/❌

4.4 REGRESSION RESULTS                             (~800 từ)
    → TABLE 6: THE KEY TABLE — 4 columns = 4 nested models
    
    TABLE 6: DETERMINANTS OF MISPRICING
    ┌────────────────────┬──────────┬──────────┬──────────┬──────────┐
    │                    │ Model 1  │ Model 2  │ Model 3  │ Model 4  │
    │                    │ Micro    │ +Manip.  │ +Macro   │ +Geo     │
    ├────────────────────┼──────────┼──────────┼──────────┼──────────┤
    │ TTM                │ X.XX***  │ X.XX***  │ X.XX***  │ X.XX***  │
    │ Volatility         │ X.XX***  │ X.XX**   │ X.XX**   │ X.XX*    │
    │ ln(Volume)         │ -X.XX*** │ -X.XX*** │ -X.XX*** │ -X.XX**  │
    ├────────────────────┼──────────┼──────────┼──────────┼──────────┤
    │ Expiry_Window      │          │ X.XX***  │ X.XX***  │ X.XX***  │
    │ Abnormal_Volume    │          │ X.XX*    │ X.XX*    │ X.XX     │
    ├────────────────────┼──────────┼──────────┼──────────┼──────────┤
    │ ΔRate_SBV          │          │          │ X.XX**   │ X.XX**   │
    │ ΔUSDVND            │          │          │ X.XX***  │ X.XX**   │
    │ Foreign_NetSell    │          │          │ X.XX**   │ X.XX*    │
    ├────────────────────┼──────────┼──────────┼──────────┼──────────┤
    │ VIX                │          │          │          │ X.XX***  │
    │ GPR                │          │          │          │ X.XX*    │
    ├────────────────────┼──────────┼──────────┼──────────┼──────────┤
    │ R²                 │ 0.XX     │ 0.XX     │ 0.XX     │ 0.XX     │
    │ Adj. R²            │ 0.XX     │ 0.XX     │ 0.XX     │ 0.XX     │
    │ F-test (vs prev.)  │          │ X.XX***  │ X.XX***  │ X.XX**   │
    │ Observations       │ 2000     │ 2000     │ 2000     │ 2000     │
    └────────────────────┴──────────┴──────────┴──────────┴──────────┘
    *p<0.10, **p<0.05, ***p<0.01. Newey-West HAC standard errors.
    
    → Interpret mỗi model: "Adding manipulation variables increases 
      R² from X to Y (F-test significant), suggesting..."
    → H6-H8 results

4.5 ROBUSTNESS CHECKS                              (~300 từ)
    → Table 7 (hoặc Appendix): Alternative specifications
    → "Results remain qualitatively unchanged when..."
    → Nếu kết quả THAY ĐỔI → giải thích tại sao (interesting!)
```

### Nguyên tắc viết Results

1. **Table trước, Text sau** — Present table → interpret key findings → DON'T repeat every number
2. **Pattern > Individual coefficients** — "Across all four models, volatility remains significant..." 
3. **Significance stars** — Dùng */**/*** cho 10%/5%/1%
4. **Nested model comparison** — Show R² tăng khi add each group → F-test cho incremental explanatory power
5. **Figures cho trends, Tables cho numbers** — Time series of mispricing → figure. Regression coefficients → table.

---

## 5. DISCUSSION (~800-1,200 từ)

### Cấu trúc

```
5.1 THEORETICAL IMPLICATIONS                       (~300 từ)
    → Findings support/challenge cost-of-carry theory?
    → Extends limits-to-arbitrage literature
    → Contribution to frontier market efficiency debate
    → "Our findings are consistent with / contrast with [author]..."

5.2 COMPARISON WITH GLOBAL EVIDENCE                 (~300 từ)
    → VN mispricing vs. MacKinlay (1988): S&P 500
    → VN mispricing vs. Samarakoon (2025): 16 markets
    → Where does VN fit in the spectrum? (developed → emerging → frontier)
    → Why different? (structural reasons)

5.3 PRACTICAL IMPLICATIONS                          (~300 từ)
    → For traders: arbitrage strategies, when opportunities exist
    → For regulators: manipulation evidence → policy recommendations
    → For UBCKNN/HNX: improve settlement mechanism? 
      Relax short-selling? Reduce transaction costs?
    → For FTSE/MSCI reclassification: market efficiency matters

5.4 POLICY IMPLICATIONS                            (~200 từ)
    → Short-selling reform
    → Settlement price calculation method
    → Transaction cost reduction
    → Market surveillance for expiry-day manipulation
```

### Sai lầm trong Discussion
- ❌ Lặp lại Results (đã nói ở Section 4)
- ✅ **Interpret** — kết quả NGHĨA LÀ GÌ cho theory và practice?
- ❌ Overclaim — "This proves that manipulation exists"
- ✅ Hedge — "Our findings provide *indirect evidence consistent with* manipulation"
- ❌ Không connect back to literature
- ✅ So sánh explicit: "Unlike MacKinlay (1988) who found X, we find Y, likely because..."

---

## 6. CONCLUSION (~600-800 từ)

### Cấu trúc

```
Đoạn 1: RECAP mục tiêu + method (2-3 câu)
    "This study examined... using... over the period..."

Đoạn 2: KEY FINDINGS (3-4 bullet points, CÓ SỐ)
    "Our analysis yields several key findings. First, ... 
    Second, ... Third, ... Fourth, ..."

Đoạn 3: IMPLICATIONS (2-3 câu)
    "These findings have important implications for..."

Đoạn 4: LIMITATIONS (2-3 câu, THÀNH THẬT)
    "This study is subject to several limitations. First, ...
    Second, ..."
    
    Limitations phổ biến:
    → Daily data (không có intraday)
    → Single market (VN only)
    → Dividend yield estimation uncertainty
    → Cross-sectional design (no causality claim)

Đoạn 5: FUTURE RESEARCH (2-3 câu)
    "Future research could extend this work by..."
    
    Ideas:
    → Intraday data for tick-by-tick mispricing
    → Covered warrants mispricing (related product)
    → Compare with other frontier markets
    → Machine learning for mispricing prediction
    → Impact of FTSE/MSCI upgrade on mispricing
```

### Lỗi phổ biến trong Conclusion
- ❌ Introduce new information/findings
- ❌ Quá dài (>1,000 từ)
- ❌ Không có limitations (reviewer sẽ add cho bạn — tốt hơn tự viết)
- ❌ Future research quá vague ("more research is needed")
- ✅ Specific: "Intraday tick data could reveal whether mispricing persists at sub-minute frequencies"

---

## REFERENCES — Format

### Nguyên tắc
- Dùng **reference manager**: Zotero (free) hoặc Mendeley (free)
- Follow journal's citation style (Emerald = Harvard, Elsevier = APA/numbered)
- **50-70 references** cho paper 7,000-9,000 từ
- Cite **gần đây** (>50% refs trong 5 năm gần nhất)
- Cite **từ target journal** (reviewer thường là editorial board member)

### Phân bổ references

| Nhóm | Số refs | Ví dụ |
|------|---------|-------|
| Core theory (cost-of-carry, arbitrage) | 8-10 | Cornell 1983, MacKinlay 1988 |
| Emerging market mispricing | 8-10 | Samarakoon 2025, Białkowski 2008 |
| Vietnam derivatives | 6-8 | 6 papers đã tìm |
| Manipulation / expiry effects | 5-7 | Stoll & Whaley 1987 |
| Geopolitical risk | 5-7 | Caldara & Iacoviello 2022 |
| Macro & financial markets | 5-7 | Baker et al. 2016 |
| Methodology | 3-5 | Newey-West 1987, Hair et al. |
| General finance/markets | 5-10 | Background context |

---

## TABLES & FIGURES — Quy tắc

### Tables
- Đánh số: **Table 1, Table 2, ...**
- Title **phía trên** table
- Notes/Sources **phía dưới** table
- Significance: *p<0.10, **p<0.05, ***p<0.01
- Standard errors/t-stats trong ngoặc đơn
- **Maximum 8-10 tables** (thừa → move to Appendix)

### Figures
- Đánh số: **Figure 1, Figure 2, ...**
- Title **phía dưới** figure
- **High resolution** (300 DPI minimum)
- **Grayscale-friendly** (nếu journal print B&W)
- **Maximum 5-6 figures**

### Expected Tables & Figures cho bài VN30

```
TABLES:
Table 1: Summary Statistics
Table 2: Variable Definitions & Sources
Table 3: Mispricing by Subperiod
Table 4: Arbitrage Boundary Violations (Upper vs. Lower)
Table 5: Expiry-Day Anomaly (t-test)
Table 6: Regression Results (4 Nested Models) ← KEY TABLE
Table 7: Robustness Checks
Table 8: Logistic Model (Boundary Violation Probability)

FIGURES:
Figure 1: Time Series of VN30F Mispricing (bp), 2017-2026
Figure 2: Distribution of Mispricing (Histogram)
Figure 3: Average Mispricing by Day-to-Expiry
Figure 4: Rolling 60-day Mispricing with VIX Overlay
Figure 5: Mispricing Comparison: VN30 vs. Global Benchmarks
```

---

## COVER LETTER — Khi Submit

```
Dear Editor,

We are pleased to submit our manuscript entitled "[Title]" 
for consideration in [Journal Name].

[1-2 câu: what the paper does]

[1-2 câu: why it fits this journal]

[1 câu: confirmation of originality]
"This manuscript has not been published or submitted elsewhere."

[1 câu: no conflicts of interest]

We look forward to your consideration.

Sincerely,
[Name], CFA, MBA
[Affiliation]
[Email]
```

---

## CHECKLIST TRƯỚC KHI SUBMIT

### Content
- [ ] Abstract có đủ 5 phần (context, method, findings với số, implications)?
- [ ] Introduction có gap rõ ràng dẫn đến RQs?
- [ ] Mỗi hypothesis có justification từ literature?
- [ ] Methodology đủ chi tiết để replicate?
- [ ] Results tables có significance stars, std errors, model fit?
- [ ] Discussion không lặp Results — interpret & compare?
- [ ] Conclusion có limitations + future research?

### Format
- [ ] Word count trong giới hạn journal?
- [ ] References format đúng journal style?
- [ ] Tables/Figures đánh số đúng, title đúng vị trí?
- [ ] Equations đánh số?
- [ ] JEL codes có?
- [ ] Keywords có?
- [ ] Cover letter có?

### Quality
- [ ] Proofread English (dùng Grammarly Premium hoặc nhờ native speaker)?
- [ ] Tất cả claims có citation?
- [ ] Không overclaim ("proves" → "suggests," "provides evidence consistent with")?
- [ ] Cite ≥3-5 papers TỪ target journal?
- [ ] ≥50% references trong 5 năm gần nhất?

---

*Hướng dẫn tạo: 2026-04-15*
*Áp dụng cho: Emerging Markets Review, RIBAF, và các Q1 finance journals*
