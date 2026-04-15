JEL Classification: G10, G19

Quy Vo,
School of Economics, Finance, and Accounting,
International University, Vietnam National University Ho Chi Minh City [https://orcid.org/0000-0001-9933-9300](https://orcid.org/0000-0001-9933-9300)

Hanh Trang Tran,
School of Economics, Finance, and Accounting,
International University, Vietnam National University Ho Chi Minh City

THE CORRELATION OF THE VOLATILITY OF FUTURE MARKET AND STOCK MARKET-A STUDY IN VIETNAM WITH 2 STAGES: COVID-19, AND GEOPOLITICS - UKRAINE INVASION

Received 15 June 2023; accepted 27 June 2023; published 03 July 2023

Abstract. Since the Vietnamese derivatives market was established, futures contracts as the representative financial instrument trading in the derivatives market. The research investigates the correlation between the spot market and the futures markets in Vietnam in which VN30 and VN30 Futures Index was chosen as research sample. Additionally, the deposit interest rate with different terms was also involved to declare the correlation between these two markets. The ARMA/GARCH model was employed to examine the volatility of the spot market, futures market, and the deposit interest rate (overnight, spot week, one-month, three-month,sixmonth,nine-month). The VAR model was employed next step to explore the correlation as well as the impact on each other. The results indicate that the tight relationship between the futures and the spot market while a negative relationship between the deposit interest rate and the spot/future market was found Especially, the examining term has been divided into 2 special stages: the Global Health Crisis (Covid-19: 2020-2021) and the Geopolitics-Ukraine invasion (2022-present) to clearly observe the correlation among three research factors.

Keywords: Volatility, Spot Market, Future Market, ARMA/GARCH,VAR,Covid-19, Geopolitics-Ukraine invasion.

In August 2017, the VN30 future contracts were officially traded with the base VN30 index. A lot of existing paper indicated the two-side impact in both positive and negative aspects between the underlying stock markets versus derivative markets in which available for trading in Vietnam is future markets. The report from Vietnam National Institute for Finance (Vu Chi Dung, 2022)

Vietnamese stock market is considered one of the frontier markets but in 2022, Vietnam has outperformed with the GDP growth rate of 8.02% (VNA, 2023), the remained one-number inflation (4.31%, tradingeconomics). By the end of February 2023, the record of Vietnam domestic stock trading accounts demonstrated nearly seven million accounts including both individual and proprietary. The amount only counted for 7 percent of total Vietnamese population while many assessments have been made and considered that the market of Vietnam as a potential market based on GDP, inflation rate, and especially stock market and worth for investment since the valuation via P/E index is quite affordable.

Introduction Background Research clearly stated the expression of this interrelationship based on five main aspects: (i) Derivatives markets contribute to the efficiency of price formation on the underlying stock markets; (ii) The liquidity of the underlying equities markets is promoted by the derivatives markets; (iii) Underlying stock markets bring condition to a better performance of derivatives markets and for investors in hedging portfolio and seeking for profit; (iv) Derivatives markets can be used to manipulate the underlying stock markets and vice versa; (v) The consequence of the derivative markets break can affect directly the underlying equities markets and the whole financial system. On the other hand, from 2018 to 2021, a downward trend was recorded about the Vietnam deposit rates due to the implementation of monetary policies with the purpose of reducing the interest rate to stimulate economic growth. Then, in 2022, the rate soared up significantly due to the rise of inflation and attracted a large amount of money.

Research Problem

While a lot of newspapers mentioned the significant rise of the deposit interest rate, the remarkably fall of the VN30 Index and the Futures trading volatility simultaneously was also noticed and reported by plenty of financial channels, newspaper ( [https://vnexpress.net/](https://vnexpress.net/)). This inverse effect raised a question that whether the deposit interest rate affects the volatility of the spot/futures markets and whether the relationship between the two markets is highlighted clearly by the volatility of deposit interest rate? Since year 2005, Vietnamese stock market has suffered chronological events that affected directly on its volatility which are the Global Financial Crisis (GFC) in 2007-2008, pre and post - Covid-19 (2020-2021), and the Russo-Ukraine war. The emergence of these events led to the fall of the market and reflected the fear of investors and the risks that the stock market may face. Limited research exists on the impact of Ukraine invasion on Vietnam's stock market volatility compared to studies on the effects of GFC, pandemic, and geopolitical events on global stock market. This study aims to investigate the market volatility and the correlation among these markets under three events objectively.

The expectation of this research would be about the strongly emphasizing on the two-way impacts from the underlying market and futures market through the results of the applied models. Also, the findings from VAR model and relating analyses may help in declaring the role of futures trading in price discovery for the underlying asset in the spot market. Moreover, the findings may bring about meaningful implications to potential investors.

Literature Review

1.1. Relevant Theoretical Frameworks

The linkage between the underlying market and the futures market, and the impact of the deposit interest rate on these markets can be explained by the arbitrage pricing theory developed by the economist Stephen Ross in 1976. The theory implies that investors can generate a risk - free profit by exploiting price discrepancies between two or more markets. The highlighted point is the possibility of arbitrage when the futures price of an asset is remarkably above its spot price. Statistical arbitrage deals with simplest financial instruments like stocks, futures, and currencies (John C. Hull, 2002; Ernest P. Chan, 2021). The relationship between the deposit interest rate and the stock market return or index can be explained based on financial intermediation theory and asset pricing model. According to Financial Intermediation Theory, the deposit interest rate and stock market are interconnected through the functioning of financial institutions. Stock market investments can be a portion of deposits (Anjan V. Thakor & Arnoud W. A. Boot, 1960). Expected returns, risk considerations, and regulatory requirements are considered as factors influencing investing in stock decisions. Higher interest rates may encourage saver to deposit more

$$
E R \_ {i} = R \_ {f} + \\beta\_ {i} \\left(E R \_ {m} - R \_ {f}\\right)
$$ measured as government bond yields, or the deposit interest rates often approximated by this short term yields. Obviously, the changes in the risk - free rate can impact on the investor's required returns and their tendency when investing in stock. Furthermore, the Monetary Policy and Interest Rate Changes theory was applied to engage the relationship between the deposit rate and the stock market. The theory suggests that the rise or fall of the interest rate by the central banks in managing inflation or stimulate economic growth, it can have ripple effect on future/spot markets. In specific higher deposit rates may attract more funds, potentially reducing liquidity in the markets and affecting the future as well as the underlying stock market prices and vice versa. As those theories implied about the fluctuations of the deposit rate impact on the stock market that involved the investor's behavior while making decisions on investments. Thus, the Portfolio theory and the Expectation theory can be applied to reinforce the frameworks for the relationship between the deposit interest rate and the spot as well as future market. Harry M. Markowitz (1959) introduced portfolio theory and the concept of diversification. In this context, the deposit rate can be viewed as a low-risk investment option, while the future or spot markets

Table 1

Vietnamese Deposit Interest Rate

|  | overnight | spot week | 1-month | 3-month | 6-month | 9-month |
| --- | --- | --- | --- | --- | --- | --- |
| 25/04/2023 | 5.07 | 5.14 | 5.56 | 7.46 | 8.33 | 8.6 |
| 31/12/2022 | 2.81 | 5.08 | 8.17 | 9.09 | 10.91 | 9.61 |
| 31/12/2021 | 0.81 | 1.93 | 3.8 | 3.68 | 3.74 | 3.26 |
| 31/12/2020 | 0.15 | 0.26 | 0.42 | 2.33 | 3.44 | 3.08 |
| 31/12/2019 | 1.52 | 2.27 | 3.53 | 4.06 | 5.11 | 5.86 |
| 31/12/2018 | 3.91 | 4.16 | 4.85 | 5.6 | 6.2 | 5.2 |

\*Source: Database of Thompson Reuters

The correlation between the deposit rates and market price could reflect the investors' preferences for risk allocation and their decisions to reallocate funds between these different investment options. The expectations theory states that the spot prices should be equal to the expected future spot price implied by the current futures price and the interest rate (Zvi Bodie et al., 2021). If the future price is higher than the spot price, a suggestion is presented that the investors are attracted to the spot price for an increase in the future, and vice versa.

The relationship between the underlying market and the futures market was examined by plenty of empirical results. Becketti & Dan J. Roberts (1990) concluded that stock index future has not increased stock market volatility whether measured by frequency or the size of large swings in stock price. According to Don M. Chance & Robert Brooks (2000), the derivatives instruments' performance depends on how other financial instruments perform. Several research has indicated the two-sided relationship in both positive and negative aspects of the stock markets and derivative markets (Kang et al., 2013, Carpenter & Whitelaw, 2017). Derivative instruments exist based on underlying securities. They reflect the change of underlying asset prices, and the future contracts reflect the investors' expectation on the equities market in future. Thus, this relationship has a close linkage and impact on each other.

There is an array of research that can be taken as examples, with the findings on the negative relationship between interest rate and stock return or stock price. They (Bhuiyan & Chowdhury, 2020; Humpe & P. Macmillan, 2007; Phuyal, 2016; Shahnaz Mashayekh et al., 2011) both conclude about the relationship and these findings also guarantee the consistency with Dividend Discount Model.

1.4. The relationship between deposit interest rates and the spot/future markets

There were plenty of papers that indicated the correlation between the spot markets and the futures trading activity, or the stock market and the deposit interest rate such as Kumar (2009) and Sehgal et al.,(2012). They illustrated a positive dynamics relationship between the spot market and the futures trading activity. Froot (1989) confirmed that a large part of the variance of excess stock returns is attributable to changing expectations of future excess stock returns. Campbell & Ammer, (1993) explored the correlation between stock returns, bond returns, and interest rates to shed light on the broader relationship between financial markets and interest rates.

1.5. Studies on Market's Volatility During Each Type of Events

The impact of pandemic has been found through several research from other countries as we understand that Covid-19 nearly hit the global. Nigeria's stock market performance can be taken as an example (Akinbobola, T.O., et al., 2022). Nguyen & Nguyen, (2022) applied the copula method to analyze the impact of Covid-19 pandemic and pointed out the dependence between the two stock market: China (Shanghai Stock Exchange) and Vietnam (Vnindex). In addition, the impact of Ukraine invasion on global finance has been reported and rated at a high - intensity level. Several studies also examined the influences as well as the afterward effects on the global financial market (Izzeldin et al., 2023), on macroeconomic aspects such as bilateral trade, oil prices, etc. within Vietnam (Randall Puah, 2022), following the invasion.

1.6. Model Hypotheses

Based on related theories and empirical evidence presented above, we hypothesized that reviewing existing literatures from these mentioned above papers, publications, as well as books, the research hypotheses have been developed as below:

H1: There is a significant correlation among the spot market, futures market, and deposit interest rate.

Methods

2.1. Data Collection

The data was collected for the main variables in the study which are the closing price of the underlying market VN30 Index and future market based on monthly contracts that was issued since 2017. The VN30 future index presented by the VN30F1M's closing price as the observation shows more effective with one that short-term duration rather than a long term contract based on the theory that the intrinsic value of the short term contract is larger than the one has large time value then. Moreover, for the deposit interest rate, the data was collected with a variety of deposit terms which are: overnight, one week, one month, three month, six month, and nine month deposit rate. Noticeably, due to the limitation in interest rate collection, there was only data since august, 2018, the range time was reset again which was from August 2018 to April 2023. Additionally, we compared the collected data from the Thompson Reuters with the State Bank of Vietnam government website to confirm the limitation of the data. The subperiod is consisted of the Global Health Crisis (2020-2021), and the Ukraine invasion (February 202

Overall, by Table 2 with the descriptive result about the dataset, it is obvious to observe that the mean of variables which is measure in return (RVN30, RVN30F, Ream..., Reninmrate) are positive and small except the negative mean of return on three-month deposit interest rate. In terms of standard deviation, the return on the futures market seems the lowest one compared to other return.

Table 2 Descriptive Statistics

| Variable | Obs | Mean | Std. dev. | Min | Max | Skewness test | Kurtosis |
| --- | --- | --- | --- | --- | --- | --- | --- |
| RVN30 | 1420 | 0.0003111 | 0.1087803 | -0.37743 | 0.4457874 | 0.08845 | 3.73904 |
| RVN30F | 1418 | 0.0000966 | 0.0068994 | -0.0314938 | 0.0294892 | -0.49453 | 7.04078 |
| Reamrate | 1420 | 0.0002901 | 0.1035232 | -0.6933901 | 0.7160033 | -0.17156 | 15.71410 |
| Reonrate | 1420 | 0.0007438 | 0.0688337 | -0.60206 | 0.4978059 | 0.17213 | 20.64087 |
| Resw | 1420 | 0.0006636 | 0.0770546 | -0.7704644 | 0.7819442 | 0.07401 | 21.78441 |
| Rethrmrate | 1420 | -0.0000241 | 0.074083 | -0.3881802 | 0.4493909 | -0.04569 | 9.55345 |
| Resixmrate | 1420 | 0.0001934 | 0.060842 | -0.4461313 | 0.3973236 | -0.06084 | 10.16269 |
| Reninmrate | 1420 | 0.0001578 | 0.0344376 | -0.2233834 | 0.2347233 | -0.04442 | 14.41892 |
| VN30 | 1420 | 1058.893 | 240.227 | 610.76 | 1572.46 | 0.72177 | 2.31466 |
| vn30fcp | 1420 | 1056.097 | 241.4242 | 578.7 | 1568 | 0.69767 | 2.32359 |
| Spotrate | 1420 | 2.28557 | 1.783058 | 0.13 | 9.48 | 0.84270 | 2.75630 |
| onrate | 1420 | 2.08207 | 1.744363 | 0.1 | 8.44 | 0.81718 | 2.61776 |
| onemrate | 1420 | 2.996077 | 1.984277 | 0.25 | 10.88 | 1.05804 | 4.00408 |
| thrmrate | 1420 | 3.861451 | 1.951418 | 0.82 | 11.8 | 1.22209 | 4.74740 |
| Sixmrate | 1420 | 4.752627 | 1.878599 | 1.21 | 12.14 | 1.48838 | 5.33770 |
| ninemrate | 1420 | 5.0495 | 1.828922 | 2.26 | 13 | 2.00712 | 7.98627 |

\*Source: Author's elaboration

On the other hand, return on all deposit interest rate shows quite high kurtosis (in range 9- 22). Generally, the Kurtosis value of all the return is higher than 3, implying that the tailedness of return margin is long and thick, and not following any of normal distribution rule.

Table 3

|  |  | Dickey-Fuller Crit.Value |  |  |
| --- | --- | --- | --- | --- |
| Variable | Test Statistic | 1% | 5% | 10% |
| RVN30 | -51.525 | -3.43 | -2.86 | -2.57 |
| RVN30F | -43.194 | -3.43 | -2.86 | -2.57 |
| Reamrate | -52.605 | -3.43 | -2.86 | -2.57 |
| Reonrate | -34.029 | -3.43 | -2.86 | -2.57 |
| Resw | -45.32 | -3.43 | -2.86 | -2.57 |
| Resixmrate | -52.335 | -3.43 | -2.86 | -2.57 |

As the dataset has the gap so the stationary checking was tested by Augmented Dickey-Fuller test. The result showed that the dataset has guaranteed its stationary condition.

2.3.1. The ARIMA regression: The ARMA/GARCH model was employed after running regression tests for the dataset to confirm there is no multicollinearity but the existence of heteroskedasticity. By applying GARCH, the volatility clustering and heteroskedasticity are captured. Moreover, GARCH model, according to (Zivot, 2009), is more advantageous than the ARCH model in estimating the random fluctuation of residuals from ARMA model.

(1)

$$
R \_ {\\mathrm {i t}} = \\log \\left(\\frac {C P \_ {\\mathrm {i t}}}{C P \_ {\\mathrm {i , t - 1}}}\\right)
$$

In which: $ CP\_{\\mathrm{i t}} $ represents the closing price of index at time t, $ R\_{\\mathrm{i t}} $ is the change in index i at time t.

$$
C P \_ {\\mathrm {i t}}
$$

$$
R \_ {\\mathrm {i t}}
$$

* * *

The optimal lag length for AR (r) and MA (s) used in this model were determined by using ACF and PACF indices.

$$
\\left(1 - \\sum\_ {i = 1} ^ {t} \\beta\_ {i} B ^ {i}\\right) R \_ {t} = \\left(1 + \\sum\_ {i = 1} ^ {S} \\gamma\_ {i} B ^ {i}\\right) \\varepsilon\_ {t}
$$

(2)

In which: the backshift operator is $ B^{i} $ . $ \\beta\_{i} $ and $ \\gamma\_{i} $ are the coefficients from the ARMA model (the AR and MA parts). The residual is represented by $ \\varepsilon\_{t} $ . After running the model, the Ljung-Box portmanteau （Q）test was applied to confirm the ARCH effect for the dataset. The expectation in this study is that the residual would be independently and identically distributed.

$$
B ^ {i}. \\beta\_ {i}
$$

$$
\\gamma\_ {i}
$$

$$
\\varepsilon\_ {t}
$$

(3)

$$
Q = n (n + 2) \\sum\_ {j = 1} ^ {m} \\frac {1}{n - j} p ^ {2} (j) \\rightarrow x \_ {m} ^ {2}
$$

m : the degree of freedom to model stationarity's test.

$$
p ^ {2} (j)
$$

$ p^{2} ( j ) $ : the estimated autocorrelation of lag j.

As the null hypothesis (H0) for expectation the series follows a white noise process, implying no ARCH effects was rejected when the Ljung-Box test indicated the p-value higher than 5%. Thus, the research jumped to the next step which is the application of ARMA(r,s)-GARCH (p, q) model to eliminate the conditional variance of VN30 future.

$$
\\widetilde {\\sigma} ^ {2} = \\alpha\_ {0} + \\sum\_ {i = 1} ^ {q} \\beta\_ {i} \\varepsilon\_ {t} + \\sum\_ {i = 1} ^ {p} y \_ {i} \\sigma\_ {t - i} ^ {2}
$$

(4)

2.3.2. The application of the forecast error variance decomposition in the market volatility spillover estimation with VAR-a vector autoregression model: The VAR model is employed in examining the relationship among variables in the model with their market indices. Then, the optimal lag length was estimated by using AIC, HQIC, and SBIC indices and two lags for models with control variables have been indicated to be suitable for the VAR application.

The VAR model: $ \\Delta Y\_{t}=\\alpha+\\beta\_{1}\\Delta Y\_{t-1}+\\beta\_{2}\\Delta Y\_{t-2}+\\dots+\\beta\_{p}\\Delta Y\_{t-p}+\\varepsilon\_{t} $

$$
\\Delta Y \_ {t} = \\alpha + \\beta\_ {1} \\Delta Y \_ {t - 1} + \\beta\_ {2} \\Delta Y \_ {t - 2} + \\dots + \\beta\_ {p} \\Delta Y \_ {t - p} + \\varepsilon\_ {t}
$$

Where:

$ Y\_{t}=Y\_{1 t},Y\_{2 t},\\dots,Y\_{n t} $ : Endogenous variables

$$
Y \_ {t} = Y \_ {1 t}, Y \_ {2 t}, \\dots , Y \_ {n t}
$$

$ \\beta\_{i} $ : Matrix with coefficients associated to lag i

$$
\\beta\_ {i}
$$

$ \\alpha : $ Vector with coefficients associated to the intercepts.

$$
\\varepsilon\_ {t}
$$

Table 4

Lagrange - Multiplier Test & Jarque - Bera tes

| Equation | Chi2 | Df | Prob>Chi2 |
| --- | --- | --- | --- |
| VN30 | 832.86 | 2 | 0.00000 |
| Vn30fpc | 6.60E+05 | 2 | 0.00000 |
| Spot Week Rate | 1.30E+04 | 2 | 0.00000 |
| Onrate | 5590.382 | 2 | 0.00000 |
| Onemrate | 1274.64 | 2 | 0.00000 |
| Sixmrate | 214.193 | 2 | 0.00000 |
| Ninemrate | 5478.988 | 2 | 0.00000 |
| All | 6.90E+05 | 14.00 | 0.00000 |

$ \\varepsilon\_{t} $ : Vector with innovations.

* * *

Although the VAR stability test showed all variables under the entire period and geopolitics event satisfied the VAR condition, when conducting VAR model for variables under the sub-period - Covid-19, the var model is unstable due to the instability of VN30 index and VN30 future index variables. Thus, Var is conducted with difference of order 1 of these two variables. Moreover, after running VAR and conducting test, the three month deposit interest rate has been eliminated to guarantee there is no autocorrelation in the equation. The result of postestimation - test is below.The Lagrange - multiplier test was conducted to assess whether there is any autocorrelation in the residual of the VAR model. At lag 2, we cannot reject the null hypothesis of no correlation since it is greater than 5 percent. Moreover, the VAR stability test showed the result that all variables satisfied the VAR conditions and lay inside the circle. The below table illustrates the VAR stability test and Granger Causality test result.

Table 5

Varstability Test

| Eigenvalue | Modulus |
| --- | --- |
| 0.9971767 | 0.997177 |
| 0.990976 | 0.990976 |
| 0.9514373 | 0.951437 |
| 0.8655907 | 0.865591 |
| 0.797424 | 0.797424 |
| 0.6221738 | 0.622174 |
| 0.5574171 | 0.557417 |
| -0.4324334 | 0.432433 |
| -0.4159855 | 0.415986 |
| -.2443302+.02016336i | 0.245161 |
| -.2443302-.02016336i | 0.245161 |
| 0.2237208 | 0.223721 |
| -0.14248 | 0.14248 |
| -0.04799673 | 0.047997 |
| All The Eigenvalues Lie Inside the Unit Circle. |  |
| VAR Satisfies Stability Condition. |  |

\*Source: Author's elaboration

By using Granger Causality, the reason impact has been illustrated obviously among tested variables. Through the Table 6, the underlying market (VN30) does not have causality relationship with the most variables while VN30, and one month deposit interest rate does great Granger cause the future market (vn30fcp). The test also illustrates that two markets (VN30, vn30fcp) do granger cause the six month deposit interest rate.

Table 6

| Equation | Excluded | Chi2 | Df | Prob>Chi2 |
| --- | --- | --- | --- | --- |
| Vn30 | Vn30fp | 4.3943 | 2 | 0.111 |
| Vn30 | Spot Week Rate | 0.49321 | 2 | 0.781 |
| Vn30 | Onrate | 0.02163 | 2 | 0.989 |
| Vn30 | Onemrate | 1.8779 | 2 | 0.391 |
| Vn30 | Sixmrate | 0.43906 | 2 | 0.803 |
| Vn30 | Ninemrate | 0.28191 | 2 | 0.869 |
| Vn30 | All | 11.943 | 12 | 0.450 |
| Vn30fp | Vn30 | 46.16 | 2 | 0.0000 |
| Vn30fp | Spot Week Rate | 0.62359 | 2 | 0.7320 |
| Vn30fp | Onrate | 0.46758 | 2 | 0.7920 |
| Vn30fp | Onemrate | 5.0227 | 2 | 0.0810 |
| Vn30fp | Sixmrate | 0.34423 | 2 | 0.8420 |
| Vn30fp | Ninemrate | 0.34556 | 2 | 0.8410 |
| Vn30fp | All | 57.789 | 12 | 0.0000 |

Granger Causality Test

* * *

| Onrate | Vn30 | 0.19119 | 2 | 0.909 |
| --- | --- | --- | --- | --- |
| Onrate | Vn30fcp | 0.02521 | 2 | 0.987 |
| Spot Week Rate | Vn30 | 0.15301 | 2 | 0.926 |
| Spot Week Rate | Vn30fcp | 0.11168 | 2 | 0.946 |
| Onemrate | Vn30 | 3.4727 | 2 | 0.176 |
| Onemrate | Vn30fcp | 4.1642 | 2 | 0.125 |
| Sixmrate | Vn30 | 7.9857 | 2 | 0.018 |
| Sixmrate | Vn30fcp | 10.611 | 2 | 0.005 |
| Ninemrate | Vn30 | 4.2073 | 2 | 0.122 |
| Ninemrate | Vn30fcp | 0.4012 | 2 | 0.818 |

\*Source: Author's elaboration

This test analysis is performed by fitting the vector autoregressive model (VAR) to the time series with L time lags as below:

Let $ X ( t ) \\in R^{d x 1} $ for $ t=1,\\ldots,t $ be a dimensional multivariate time series.

$$
X (t) \\in R ^ {d x 1}
$$

$$
t = 1, \\dots , t
$$

$$
X (t) = \\sum\_ {\\tau = 1} ^ {L} A \_ {\\tau} X (t - \\tau) + \\varepsilon (t)
$$

In which: $ \\varepsilon (t) $ is a white Gaussian random vector, $ A\_{\\tau} $ is a matrix for every $ \\tau $ . A time series $ X\_{i} $ is called a Granger cause of another time series $ X\_{j}. $

$$
X \_ {i}
$$

$$
X \_ {j}
$$

Finally, the impulse and response functions are used with applying the Cholesky forecast error variance decomposition.

Results

3.1. Estimating The Market Volatility Using ARMA/GARCH

Table 7 below presents the estimated results for entire period (08.2018-04.2023) which illustrated the ARCH-GARCH effects existed in all variables. It implied that the the market volatilities are affected by both volatilities and shocks from events in previous period. The results also were presented by variance constant graph to show the market volatilities across the variables.

Table 7

Volatility in the entire period (2018-4/2023

| Variance Equation | RVN30 | RVN30F | Reamrate | Resw | Reonrate | Re3mrate | Resixmrate | Reninmrate |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| ARCH(α) | 0.134\*\*\* | 0.331\*\*\* | 0.481\*\*\* | 0.499\*\*\* | 0.534\*\*\* | 0.564\*\*\* | 0.161\*\*\* | 0.0863\*\*\* |
|  | (0.0396) | (0.0311) | (0.0344) | (0.0454) | (0.0339) | (0.0389) | (0.0275) | -0.0114 |
| GARCH(β) | 0.553\*\*\* | 0.618\*\*\* | 0.784\*\*\* | 0.547\*\*\* | 0.292\*\*\* | 0.462\*\*\* | 1.187\*\*\* | 1.446\*\*\* |
|  | (0.20) | (0.04) | (0.03) | (0.0288) | (0.0203) | (0.0376) | (0.1120) | -0.0386 |
| Constant | 0.00292\* | 0.00000126 | -0.00121\*\*\* | 0.000052 | 0.00133\*\*\* | 0.000330\*\*\* | -0.00100\*\*\* | -0.000604\*\*\* |
|  | (0.001720) | (0.000001) | (0.000142) | (0.000063) | (0.000078) | (0.000092) | (0.000292) | -0.0000352 |
| (α+β) | 0.68700 | 0.9490000 | 1.26500 | 1.04600 | 0.82600 | 1.02600 | 1.34800 | 1.5323 |
| Standard errors in parentheses |  |  |  |  |  |  |  |  |

The row of $ (\\alpha+\\beta) $ indicates the mean -reversion speed process of each variable. The number showed the value which is smaller than 1 has mean -reversion progress and the smaller value is, the faster the process is. Thus,the results show overnight rate has mean -reversion process (other type of deposit rate witnessed no mean-reversion) and the fastest one is VN30 index with the lowest value of 0.687 and the lowest one is VN30 futures index with value of 0.949. By this amount,it can be said that the return on VN30 futures index volatility is affected by shock in the long term.

$$
(\\beta \\text {o f} 0. 7 8 \_ {4})
$$

\*Source: Author's Elaboration

- p<0.1, \*\* p<0.05, \*\*\* p<0.01

* * *

Next, the estimation is conducted similarly to examine the volatility in two sub-periods: Covid-19 and the Ukraine invasion. The results from the two below tables also show that both volatility and shocks under these events affect the market fluctuation. These tables are presented below with the results confirm ARCH and GARCH effects to all variables.

Volatility under the Covid - 19 (2020-2021)

| Variance Equation | RVN30 | RVN30F | Reamrate | Resw | Reonrate | Re3mrate | Resixmrate | Reninmrate |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| ARCH(α) | 0.133\*\* | 0.661\*\*\* | 0.386\*\*\* | 0.545\*\*\* | 0.320\*\*\* | 1.453\*\*\* | 0.319\*\*\* | 0.0435\*\*\* |
|  | -0.0761 | -0.0811 | -0.0668 | -0.0898 | (0.0691) | (0.0755) | (0.0728) | -0.0114 |
| GARCH(β) | 0.553 | 0.230\*\*\* | 0.941\*\*\* | 0.508\*\*\* | 0.882\*\*\* | 0.0558\* | -0.133\* | 1.630\*\*\* |
|  | -0.371 | -0.0759 | -0.0779 | -0.0554 | -0.0984 | (0.0286) | (0.0723) | -0.104 |
| Constant | 0.00281 | -0.0000117\*\*\* | (-0.00332)\*\*\* | 0.000269 | -0.00103\*\* | 0.000634\*\*\* | 0.00493\*\*\* | -0.00128\*\*\* |
|  | -0.00294 | -2.82E-06 | -0.000886 | -0.000226 | -0.000518 | (0.0000824) | (0.000391) | -0.000171 |
| (α+β) | 0.686 | 0.891 | 1.327 | 1.053 | 1.202 | 1.5088 | 0.186 | 1.6735 |

Standard errors in parentheses

\*Source: Author's Elaboration

- p<0.1, \*\* p<0.05, \*\*\* p<0.01

Figure 1. Market Volatility (entire period)

\*Source: Author's Elaboration

Cond
01jan2020 01ju2020 01jan2021 01ju2021 01jan2022
Exchange Date

* * *

Figure 3. Market Volatility (2022 - 04.2023)

\*Source: Author's Elaboration

It is understandable as this is the underlying market and is affected by its consisting sector top 30 Vietnamese listed companies with the largest market capitalization. In addition, under the Covid-19 term, the future market seems to fluctuate a lot compared to the entire period. The reason behind this volatility can be explained that people accept to take risk for a high premium when other instruments (the deposit interest rate) are continuously nailed down and all other activity is locked down since the half of 2021.

3.2. The Relationship between Spot market, Future Markets, and deposit interest rate:

3.2.1. Variance Decomposition:

The variance decomposition is employed in explaining the impact of one variable on other variables and analyzing the relationship between the two markets: The futures market and its underlying market and comparing the volatility with the effect of the depositing interest rate.

For the entire period, the change of VN30 seems less likely to be explained by other variables in the impulse while the percentage of variation in the futures market explained by its underlying market of 92 percent. The results in Table 9 and Table 10 show a less likely effect of deposit interest rate on the derivatives and spot market.The granger causality test which was mentioned above also clearly stated the causality of deposit interest rate and the two markets. On the other hand, from the result, the overnight rate can explain the change in both VN30 future index and VN30 index at the highest proportion (approximately 0.7 percent) compared to other types of deposit interest rate including spot week rate, one month rate, six-month and nine-month rate.

- p<0.1, \*\* p<0.05, \*\*\* p<0.01

Standard errors in parentheses

Table 10

Variance Decomposition (Response VN30 Future) - Entire Period

Volatility in 2022-4.2023

| Impulse(VN30,Onrate,SpotWeekRate,Onemrate,Sixmrate,Ninemrate) |  |  |  |  |  |  |
| --- | --- | --- | --- | --- | --- | --- |
| Step | VN30 | SpotWeekRate | Onrate | Onemrate | Sixmrate | Ninemrate |
| 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| 1 | 0 | 0 | 0 | 0 | 0 | 0 |
| 2 | 0.788821 | 0.00033 | 0.000011 | 0.003095 | 9.30E-06 | 0.000167 |

* * *

| 3 | 0.821123 | 0.000233 | 0.000034 | 0.002308 | 0.000053 | 0.000217 |
| --- | --- | --- | --- | --- | --- | --- |
| 4 | 0.848113 | 0.000299 | 0.000077 | 0.002511 | 0.000088 | 0.000232 |
| 5 | 0.867071 | 0.000642 | 0.000074 | 0.002412 | 0.000098 | 0.000248 |
| 6 | 0.881784 | 0.001251 | 0.000064 | 0.002588 | 0.000097 | 0.000248 |
| 7 | 0.893042 | 0.002073 | 0.000064 | 0.002759 | 0.000089 | 0.000248 |
| 8 | 0.901826 | 0.00306 | 0.000093 | 0.003018 | 0.000081 | 0.000243 |
| 9 | 0.908702 | 0.004164 | 0.000164 | 0.003288 | 0.000072 | 0.000238 |
| 10 | 0.914109 | 0.00535 | 0.000284 | 0.003576 | 0.000066 | 0.000232 |
| 11 | 0.918364 | 0.006591 | 0.000455 | 0.003858 | 0.000061 | 0.000225 |
| 12 | 0.921706 | 0.007864 | 0.000679 | 0.004131 | 0.000058 | 0.000219 |

\*Source: Author's Elaboration

Table 11

Variance Decomposition (Response VN30) - entire period

| Impulse(Vn30fcp,Onrate,SpotWeekRate,Onemrate,Sixmrate,Ninemrate) |  |  |  |  |  |  |
| --- | --- | --- | --- | --- | --- | --- |
| Step | Vn30fcp | Onrate | SpotWeekRate | Onemrate | Sixmrate | Ninemrate |
| 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| 1 | 0 | 0 | 0 | 0 | 0 | 0 |
| 2 | 0.00306 | 0.000088 | 0.000185 | 0.000938 | 0.000203 | 0.000083 |
| 3 | 0.002747 | 0.000064 | 0.000295 | 0.001599 | 0.000333 | 0.000086 |
| 4 | 0.003 | 0.000242 | 0.000402 | 0.001996 | 0.000403 | 0.000089 |
| 5 | 0.002965 | 0.000663 | 0.000435 | 0.00245 | 0.000449 | 0.000093 |
| 6 | 0.002982 | 0.001297 | 0.000412 | 0.002844 | 0.000473 | 0.000097 |
| 7 | 0.002951 | 0.002089 | 0.000365 | 0.003251 | 0.000484 | 0.000101 |
| 8 | 0.002923 | 0.003 | 0.00032 | 0.003631 | 0.000486 | 0.000106 |
| 9 | 0.002887 | 0.003996 | 0.000298 | 0.003995 | 0.000482 | 0.000111 |
| 10 | 0.00285 | 0.005053 | 0.000312 | 0.004333 | 0.000474 | 0.000116 |
| 11 | 0.002814 | 0.006154 | 0.000372 | 0.004644 | 0.000464 | 0.00012 |
| 12 | 0.00278 | 0.007284 | 0.00048 | 0.004926 | 0.000452 | 0.000125 |

Briefly, the deposit interest rate is not able to explain more than 1 to 5 percent change in both spot and derivatives market. However, in Covid-19, the proportion of explanation by 1-month deposit interest rate and 6-month deposit interest rate about the variances of the two markets is nearly up to 3 percent. Moreover, in the period of 2022 now, the variance of VN30 index and VN30 Future Index can be explained approximately 2 percent by mostly deposit interest rate variable. For example, the spot week rate could explain the volatility of VN30 about 2.4 percent and explain the volatility of VN30 Future Index about 2.7 percent (Table 11-15).

Variance Decomposition (Response VN30) - Covid term

| Impulse(Vn30fcp,Onrate,SpotWeekRate,Onemrate,Sixmrate,Ninemrate) |  |  |  |  |  |  |
| --- | --- | --- | --- | --- | --- | --- |
| Step | Vn30fcp | SpotWeekRate | Onrate | Onemrate | Sixmrate | Ninemrate |
| 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| 1 | 0 | 0 | 0 | 0 | 0 | 0 |
| 2 | 0.04185 | 0.002145 | 0.005478 | 0.000314 | 0.005075 | 0.004289 |
| 3 | 0.043062 | 0.003025 | 0.009316 | 0.000382 | 0.009889 | 0.008155 |
| 4 | 0.044768 | 0.003988 | 0.009642 | 0.000534 | 0.01064 | 0.008593 |
| 5 | 0.044777 | 0.003982 | 0.009826 | 0.000697 | 0.011791 | 0.008844 |
| 6 | 0.044962 | 0.004001 | 0.009898 | 0.001289 | 0.011954 | 0.009198 |
| 7 | 0.044946 | 0.004011 | 0.010044 | 0.001351 | 0.012003 | 0.009282 |
| 8 | 0.044966 | 0.004044 | 0.010102 | 0.001506 | 0.012015 | 0.009446 |
| 9 | 0.044959 | 0.004073 | 0.010189 | 0.001536 | 0.012012 | 0.009513 |
| 10 | 0.044964 | 0.004105 | 0.010251 | 0.001584 | 0.012013 | 0.009594 |
| 11 | 0.04496 | 0.004134 | 0.010322 | 0.001603 | 0.012013 | 0.009642 |
| 12 | 0.04496 | 0.004163 | 0.010383 | 0.001622 | 0.012014 | 0.009688 |

* * *

explanation by deposit interest rate, the granger test may be misleading due to lacking in economic significance.

Table 13

Variance Decomposition (Response VN30 Future) - Covid Term

Impulse (VN30, Onrate, Spot Week Rate, Onemrate, Sixmrate, Ninemrate)

| Impulse(VN30, Onrate, Spot Week Rate, Onemrate, Sixmrate,Ninemrate) |  |  |  |  |  |  |
| --- | --- | --- | --- | --- | --- | --- |
| Step | VN30 | SpotWeekRate | Onrate | Onemrate | Sixmrate | Ninemrate |
| 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| 1 | 0.828055 | 0 | 0 | 0 | 0 | 0 |
| 2 | 0.802157 | 0.005418 | 0.023035 | 0.000079 | 0.007649 | 0.00004 |
| 3 | 0.791944 | 0.006072 | 0.022928 | 0.000412 | 0.01589 | 0.001251 |
| 4 | 0.78553 | 0.006359 | 0.022881 | 0.001779 | 0.017357 | 0.002694 |
| 5 | 0.784256 | 0.006348 | 0.023387 | 0.001797 | 0.018289 | 0.002802 |
| 6 | 0.782647 | 0.006363 | 0.023403 | 0.00256 | 0.018502 | 0.003385 |
| 7 | 0.782354 | 0.006382 | 0.023601 | 0.00259 | 0.018516 | 0.003481 |
| 8 | 0.781854 | 0.006424 | 0.023654 | 0.002772 | 0.018534 | 0.003725 |
| 9 | 0.781629 | 0.00646 | 0.023767 | 0.002803 | 0.018531 | 0.00382 |
| 10 | 0.781364 | 0.006501 | 0.023838 | 0.002864 | 0.018535 | 0.003941 |
| 11 | 0.781175 | 0.006537 | 0.023926 | 0.00289 | 0.018538 | 0.004014 |
| 12 | 0.780995 | 0.006573 | 0.023998 | 0.002918 | 0.018541 | 0.00408 |

\*Source: Author's Elaboration

Table 14

Variance Decomposition (Response VN30) - (2022-4.2023)

Impulse (Vn30fcp, Onrate, Spot Week Rate, Onemrate, Sixmrate, Ninemrate)

| Impulse(Vn30fcp,Onrate,SpotWeekRate,Onemrate,Sixmrate,Ninemrate) |  |  |  |  |  |  |
| --- | --- | --- | --- | --- | --- | --- |
| Step | Vn30fcp | SpotWeekRate | Onrate | Onemrate | Sixmrate | Ninemrate |
| 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| 1 | 0 | 0 | 0 | 0 | 0 | 0 |
| 2 | 0.022372 | 0.000114 | 0.007295 | 0.000699 | 0.000109 | 0.002746 |
| 3 | 0.020533 | 0.001301 | 0.009072 | 0.00373 | 0.000074 | 0.004043 |
| 4 | 0.018663 | 0.003262 | 0.009706 | 0.004364 | 0.000241 | 0.00577 |
| 5 | 0.017402 | 0.005395 | 0.010589 | 0.005513 | 0.000358 | 0.007056 |
| 6 | 0.016378 | 0.007883 | 0.011128 | 0.00679 | 0.000402 | 0.008427 |
| 7 | 0.01555 | 0.010526 | 0.011541 | 0.00805 | 0.000416 | 0.009687 |
| 8 | 0.01487 | 0.013283 | 0.011849 | 0.009266 | 0.000407 | 0.010896 |
| 9 | 0.014302 | 0.016111 | 0.012067 | 0.010398 | 0.000384 | 0.012049 |
| 10 | 0.013817 | 0.018983 | 0.012204 | 0.011433 | 0.000357 | 0.013153 |
| 11 | 0.0134 | 0.021878 | 0.012267 | 0.012365 | 0.000328 | 0.014211 |
| 12 | 0.013036 | 0.024781 | 0.012263 | 0.013194 | 0.000303 | 0.015227 |

\*Source: Author's Elaboration

Variance Decomposition (Response VN30 Future) - (2022-04.2023)

| Step | VN30 | Spot Week Rate | Onrate | Onemrate | Sixmrate | Ninemrate |
| --- | --- | --- | --- | --- | --- | --- |
| 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| 1 | 0.890985 | 0 | 0 | 0 | 0 | 0 |
| 2 | 0.882305 | 0.000298 | 0.005915 | 0.006377 | 6.40E-06 | 0.001834 |
| 3 | 0.896569 | 0.002394 | 0.006138 | 0.00683 | 0.000569 | 0.004119 |
| 4 | 0.9042 | 0.004615 | 0.007243 | 0.006974 | 0.001638 | 0.005684 |
| 5 | 0.907201 | 0.007191 | 0.008245 | 0.008071 | 0.002095 | 0.007184 |
| 6 | 0.907838 | 0.009978 | 0.009037 | 0.009387 | 0.002275 | 0.008559 |
| 7 | 0.907023 | 0.012832 | 0.009747 | 0.010773 | 0.002294 | 0.009799 |
| 8 | 0.905316 | 0.015717 | 0.010361 | 0.012119 | 0.002221 | 0.010951 |
| 9 | 0.90309 | 0.018602 | 0.010873 | 0.013367 | 0.002105 | 0.012029 |
| 10 | 0.900573 | 0.021469 | 0.011279 | 0.01449 | 0.001971 | 0.013049 |
| 11 | 0.897906 | 0.024307 | 0.011579 | 0.015483 | 0.001836 | 0.014022 |
| 12 | 0.895176 | 0.027111 | 0.011779 | 0.016347 | 0.001708 | 0.014954 |

Impulse (VN30, Onrate, Spot Week Rate, Onemrate, Sixmrate, Ninemrate)

* * *

Briefly, the impact of the spot market on the futures market has been confirmed strongly through the forecast error variance decomposition results in both entire period and sub-period while the futures market volatility suggest a slight impact that can be explained by this variable on the spot market. On the other hand, all types of deposit interest rates make a slight contribution to explaining the variance of the two markets.

3.2.2. Impulse Response Analysis:

After the variance decomposition analysis, the orthogonal impulse and response functions are applied next with the use of orthogonalized Impulse response functions for each market. (Sims, 1980) made suggestion about the application of these functions while analyzing the relationship and avoiding the misleading error may happen due to the lack of economic significance when only VAR model or the Granger Causality test are employed. The magnitude of the shock which is simulated by the OIRF graph corresponds to one-unit standard deviation.

The Impulse and Response function is used to analyze the impact of change in the spot market on derivatives market and vice versa. The other variables (deposit interest rate) are involved to observe the proportion of volatility on the two markets. The graphs are shown in Figure 4,5.

Figure 4. OIRF Covid term (2020 - 2021) and Geopolitics Event (2022-04.2023) \*Source: Author's Elaboration response to the change while for the rest, the slight decrease of VN30 index is illustrated on the graph. In addition, the change in the four rates including the spot week, overnight, 6 - month, 9 month deposit interest rates, in the next steps till the end stage, reflects a sharp decline and even negative reaction of the spot market. On contrast, the positive response, and a stable trend of VN30 index has been illustrated with the impulse of the future market and the one-month deposit interest rate on the graph after 5-day lags. On the other hand, for the response of VN30 future index, in very first step, the change in the spot market reflects a fall of the future market and a slight increase again in the next steps, then the stable trend is maintained till the end of stage. Additionally, except the 1-month deposit interest rate, the impulse from other deposit interest rate causes negative response of the future market.

When analyzing the volatility of the two markets under the sub-period (GHC, Ukraine invasion), the graphs look a lot more interesting. In the begin day lag in the Covid-19 term, the shock from the spot market causes a sharp decline of the future market while a significant increase in VN30 index is recorded as the response to the shock from the future market. However, in this period, after the fifth day lag, the response remains steady. In the Ukraine invasion (2022-present), except a slight increase of VN30 index as the response to the change in VN30 future and then remaining the stable trend, both two markets have negative response to the change in deposit interest rate.

The results of the OIRF (orthogonal impulse - response function) confirm once more time the findings of Granger causality and the variance decomposition analysis above. The OIRF delivers confirmation on the negative impact of the deposit interest rate volatility on the two markets and a strong effect from each market on each other.

The study investigates not only the impact of the spot market on the derivatives and vice versa, but also their volatility effects when the period is separated following the two great events that cause effects on the whole financial market. The results showed that the shock influences both markets and confirmed the hypothesis about the negative correlation between the spot as well as the future market and the deposit interest rate. Additionally, with GARCH model, the volatility of these two markets is also presented clearly and how they fluctuate during the Covid-19 and the Ukraine war term. Moreover, the findings by GARCH model in this study is like (Ho Thuy Tien et al., 2017; Nguyen Thi Hien et al., 2022) about the long - term impact on volatility by shock of the underlying market and the future market. The study of (Ray Yeutien Chou, 1988) also supports the result found by GARCH.

The study's results recommend the investors to pay attention to an effective risk management strategy as the fluctuation is demonstrated as being affected by the volatility in the past. The flexible allocation of investment is also necessary to take benefit of the market capabilities, as a rise in interest rate may lead to the fall of the stock market. Moreover, the results implied that the investor could take advantage of historical volatility in conducting market research as well as the forecast to minimize the portfolio risk and have a well - preparation before potential risk due to "black swan" events. In other words, the study encourages investors to monitor the risk exposure in both markets closely to update the insight of self - investment. As the positive correlation between the two markets implies that changes in one market are likely to influence the other. Therefore, this could be applied to build reasonable trading strategies. For example, hedging actions can be considered or taken when the investors receive any signals showing that their portfolio may suffer loss from the spot market. Other than that, the negative correlation between the two markets and the deposit interest rate implied a flexible investment is essential in building wealth, or reasonable investing strategies. However, the readers who are interested in investing also need to read the limitations of the study to consider their understanding, and their trading strategies. Those above recommendations are for reference rather than following absolutely.

As mentioned above, the study conducted while there are rare previous papers,limitations are unavoidable. In this research, due to the lack of data publications,the result of the research is validity from august 2018 rather than august 2017 - the birth of VN30 future.Moreover,the research aims to provide an overview of the correlation among three variables instead of a detailed insight rather than a detailed view.Because the relationship between deposit interest rate and the stock markets are assessed as a complex relationship in the literature review session due to the impacts from other macroeconomic factors.The time range (2018-2023) is appropriate for studying both three variables.Additionally,the study also revealed just one aspect of common investors behavior rather than the whole.In particular,the investor behavior tends to what they beneficiary such as higher interest rate,or lower risk but stable return,etc.As financial markets are complex and subject to various inefficiencies,investing decisions can be rational or irrational.The research test which has been demonstrated in the table of descriptive statistics also confirmed that the market distribution did not follow any regulations.Additionally,the scope of the study is in Vietnamese markets,so it could restrict the

Funding: This research received no external funding.

Conflicts of Interest: The authors declare that no potential conflicts of interest in publishing this work. Furthermore, the authors have witnessed ethical issues such as plagiarism, informed consent, misconduct, data fabrication, double publication or submission, and redundancy.

Publisher's Note: The European Academy of Sciences Ltd remains neutral with regard to jurisdictional claims in published maps and institutional affiliations.

References

Akinbobola, T.O., Awosoga, O.A., Babalola, C.P., Okunade, S.O., Agumadu, M.A., Shuaib, F.L. (2022). Impact Analysis of Pandemic on Nigeria's Stock Market Performance. Research in Applied Economics, 14(2), 17. [https://doi.org/10.5296/rae.v14i2.20560](https://doi.org/10.5296/rae.v14i2.20560)
Anjan V. Thakor, & Arnoud W.A. Boot (Eds.). (1960). Handbook Of Financial Intermediation And Banking. Elsevier.
Becketti, & Dan J. Roberts. (1990). Will increased regulation of stock index futures reduce stock market volatility? Economic Review - Federal Reserve Bank of Kansas City, 75(6), 33-46.
Bhuiyan, E.M., & Chowdhury, M. (2020). Macroeconomic variables and stock market indices: Asymmetric dynamics in the US and Canada. The Quarterly Review of Economics and Finance, 77, 62

* * *

Humpe, A., & P. Macmillan. (2007). Can macroeconomic variables explain long term stock market movements? A comparison of the US and Japan CDMA working. Finance , 30, 209-245.

Izzeldin, M., Muradoglu, Y.G., Pappas, V., Petropoulou, A., & Sivaprasad, S. (2023). The impact of the Russian-Ukrainian war on global financial markets. International Review of Financial Analysis, 87, 102598. [https://doi.org/10.1016/j.irfa.2023.102598](https://doi.org/10.1016/j.irfa.2023.102598)

John C Hull. (2002). Options, Futures, and Other Derivatives.

Kang, S.H., Cheong, C., & Yoon, S.-M. (2013). Intraday volatility spillovers between spot and futures indices: Evidence from the Korean stock market. Physica A: Statistical Mechanics and Its Applications, 392(8), 1795-1

$ \\textcircled{c} $ 2023 by the author(s). Submitted for possible open access publication under the terms and conditions of the Creative Commons Attribution (CC BY) license ( [http://creativecommons.org/licenses/by/4.0/](http://creativecommons.org/licenses/by/4.0/)).