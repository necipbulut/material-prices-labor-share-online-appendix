# Online Appendix to “Monetary Policy, Material Prices and the Labor Share: Evidence from Türkiye”

The full text of the Online Appendix follows, with all its tables, equations, figures and notes; the typeset version is [Online_Appendix.pdf](Online_Appendix.pdf).

**Contents**

- [OA.1 The sector panel](#oa1-the-sector-panel)
- [OA.2 The world price instrument](#oa2-the-world-price-instrument)
  - [Table OA1. Products and world prices of the instrument](#table-oa1)
- [OA.3 Further robustness checks](#oa3-further-robustness-checks)
  - [Table OA2. Real interest rate control and long difference](#table-oa2)
  - [Figure OA1. Estimates without one sector at a time](#figure-oa1)
- [OA.4 Inference](#oa4-inference)
- [OA.5 Supplier prices](#oa5-supplier-prices)
  - [Table OA3. Cumulative supplier price responses, with and without electricity and gas](#table-oa3)
- [OA.6 The lagged coefficient of Table 5](#oa6-the-lagged-coefficient-of-table-5)
  - [Table OA4. The coefficients of Table 5, column (3), by component](#table-oa4)
- [OA.7 Local projections](#oa7-local-projections)
  - [Table OA5. Local projections of the labor share](#table-oa5)
- [OA.8 Heterogeneity and the share equation](#oa8-heterogeneity-and-the-share-equation)
  - [Table OA6. Markup interaction](#table-oa6)
- [OA.9 Contributions to the labor share](#oa9-contributions-to-the-labor-share)
- [References](#references)

---

Equations, tables and figures without “OA” refer to the paper.

## OA.1 The sector panel

The panel comes from TURKSTAT’s structural business statistics for two-digit sectors (NACE Rev. 2), which leave out agriculture, finance and public administration. We also drop education, health, arts and other personal services, since the statistics miss their large public and non-profit producers. A confidential cell is recovered from the section total when it is the only one in its section and year; otherwise only the change in stocks is allocated, in proportion to output. Ten of the 63 sectors still miss some years, which leaves 719 observations.

Published value added at factor cost leaves out the change in stocks of purchased goods, so the labor share uses $`VA=VA^{pub}+\Delta S`$, with intermediate consumption $`M`$ equal to output less $`VA`$. When inflation is high, part of $`\Delta S`$ is a holding gain, so our figure is then an upper bound on value added and the published one a lower bound.

The material price index of a sector averages the log prices of 64 supplier products with the weights of its domestic and imported purchases in the 2012 input–output table. Domestic purchases are priced by TURKSTAT’s two-digit producer price indices (PPI) for industry and its agricultural and services PPI, or by value added deflators where no PPI exists, and imports by TURKSTAT’s import unit value indices in TL. The services PPI starts in 2017 and is chained back with the section’s value added deflator, and monthly and quarterly indices are averaged over the year. PPIs price 64% of purchases in the average basket.

The markup is output over intermediate consumption and personnel costs, $`\mu_{j}=R_{j}/(M_{j}+W_{j})`$, and the material share of variable cost is $`\theta_{m,j}=M_{j}/(M_{j}+W_{j})`$, both averaged over 2009–2012. On this cost base eq. (8) holds exactly, and a markup below one coincides with a labor share above one. Only employment activities (N78) have a markup below one (0.992). The cost of capital is left out, so the measured markup is an upper bound on the margin over full cost. A markup built from turnover over purchases and personnel costs averages 1.078 and falls below one in 22% of the observations. We do not use it: goods bought for resale pull it toward one, and stock building in its purchases breaks eq. (8).

The export share is exports over output, and import penetration is imports over output less exports plus imports. FX loans are foreign currency cash loans over short- and long-term liabilities; only bank loans are split by currency, so the ratio is a lower bound on a section’s foreign currency debt.

## OA.2 The world price instrument

The instrument of eq. (23) prices the 27 goods of Table OA1. We split the single mining product of the 2012 input–output table into coal, crude petroleum, natural gas, metal ores and other mining. Energy imports come from the 2012 Eurostat energy balance at world prices, and the mining purchases of each column are allocated with a RAS procedure that keeps structural zeros.

Each six-digit HS code of Türkiye’s imports is assigned to its CPA product through the correspondences from HS to CPC 2.1 and from CPC 2.1 to CPA 2.1 and ISIC Rev. 4, in the spirit of Pierce and Schott (2012). For the 24 goods with import codes, the world price of a good is a chained index of the unit values of its codes in UN Comtrade, import value in US dollars over net weight. Its annual log change is the mean log change of these codes, weighted by their 2013 imports, after changes more than $`\ln2`$ from the weighted median are dropped. The other three goods take World Bank prices. Precious metals, mostly gold that the input–output table records as re-exported, are left out of basic metals. Printing, water and services have no world price, so the weights of a sector sum to the priced share of its variable cost, 0.389 on average.

<a name="table-oa1"></a>**Table OA1. Products and world prices of the instrument**

| Product                            | Price           | HS6<br>codes | Imports<br>2013 | Weight, %<br>Mean | Weight, %<br>Largest | Log change<br>2020–2022 |
|:-----------------------------------|:----------------|-------------:|----------------:|------------------:|---------------------:|------------------------:|
| A01 Crops and livestock            | Comtrade        | 221          | 7.45            | 1.88              | 41.8 (C10–C12)       | 0.41                    |
| A02 Forestry                       | Comtrade        | 13           | 0.12            | 0.35              | 15.6 (C16)           | 0.53                    |
| A03 Fish                           | Comtrade        | 41           | 0.06            | 0.04              | 0.9 (I)              | 0.31                    |
| B05 Coal                           | Comtrade        | 3            | 0.83            | 0.27              | 6.9 (C23)            | 1.16                    |
| B06 Crude petroleum                | WB: Brent       | –            | –               | 0.00              | –                    | 0.86                    |
| B06 Natural gas                    | WB: gas, Europe | –            | –               | 0.59              | 6.1 (C20)            | 2.52                    |
| B07 Metal ores                     | Comtrade        | 18           | 1.21            | 0.72              | 7.7 (B)              | 0.40                    |
| B08 Other mining                   | Comtrade        | 55           | 0.38            | 0.44              | 9.5 (C23)            | 0.44                    |
| C10–C12 Food, beverages, tobacco   | Comtrade        | 515          | 8.25            | 1.86              | 29.8 (I)             | 0.31                    |
| C13–C15 Textiles, apparel, leather | Comtrade        | 817          | 10.31           | 2.88              | 46.0 (C13–C15)       | 0.15                    |
| C16 Wood                           | Comtrade        | 82           | 1.48            | 1.21              | 27.8 (C16)           | 0.24                    |
| C17 Paper                          | Comtrade        | 119          | 3.84            | 1.80              | 33.7 (C17)           | 0.41                    |
| C19 Refined petroleum              | Comtrade        | 18           | 20.80           | 3.38              | 32.3 (H51)           | 0.85                    |
| C20 Chemicals                      | Comtrade        | 756          | 29.12           | 4.31              | 52.6 (C20)           | 0.46                    |
| C21 Pharmaceuticals                | Comtrade        | 89           | 4.90            | 0.51              | 21.6 (C21)           | −0.07                   |
| C22 Rubber and plastics            | Comtrade        | 139          | 5.28            | 1.68              | 13.7 (C22)           | 0.14                    |
| C23 Non-metallic minerals          | Comtrade        | 158          | 2.09            | 1.55              | 18.5 (C23)           | 0.16                    |
| C24 Basic metals                   | Comtrade        | 330          | 20.30           | 4.17              | 43.5 (C25)           | 0.47                    |
| C25 Fabricated metals              | Comtrade        | 231          | 5.44            | 1.32              | 8.7 (C25)            | 0.17                    |
| C26 Electronics                    | Comtrade        | 274          | 15.53           | 1.17              | 35.8 (C26)           | 0.28                    |
| C27 Electrical equipment           | Comtrade        | 205          | 10.14           | 1.33              | 13.2 (C27)           | 0.11                    |
| C28 Machinery                      | Comtrade        | 465          | 23.77           | 0.93              | 13.1 (C28)           | 0.01                    |
| C29 Motor vehicles                 | Comtrade        | 73           | 20.27           | 0.82              | 30.0 (C29)           | 0.09                    |
| C30 Other transport equipment      | Comtrade        | 78           | 4.20            | 0.42              | 14.3 (C30)           | −0.01                   |
| C31–C32 Furniture, other goods     | Comtrade        | 200          | 4.44            | 0.49              | 10.3 (C31–C32)       | 0.10                    |
| D35 Electricity and gas            | WB: gas, coal   | –            | –               | 2.50              | 25.8 (E36)           | 2.32                    |
| E37–E39 Waste and scrap            | Comtrade        | 50           | 7.89            | 2.25              | 33.1 (E37–E39)       | 0.52                    |
| All products                       |                 | 4,840        | 208.09          | 38.85             |                      |                         |

Notes: The goods of $`Z^{f}_{jt}`$, eq. (23). Price: Comtrade, chained index of Türkiye’s import unit values (Section OA.2); WB, World Bank prices as annual averages, with gas weighted by 0.803 and coal by 0.197 for electricity and gas. HS6 codes and imports: codes with 2013 imports and their value in billion US dollars, split equally where a code maps to several products; the total counts each code once, and all of Türkiye’s 2013 imports were 260.8 billion US dollars. Weight: share in the variable cost of the sector’s input–output column, eq. (24), mean over the 63 sectors and largest value (column in parentheses); crude petroleum enters only C19, outside the sample. Log change: $`\ln P^{f}_{p,2022}-\ln P^{f}_{p,2020}`$.

## OA.3 Further robustness checks

Table OA2 adds two checks to Table B1. Low and negative real interest rates went with a weaker TL in 2017–2022 (Gürkaynak et al., 2023). Yet a control for material intensity times the real interest rate (row (2)) leaves the estimates close to the baseline, and the control itself is not significant. In the long difference over 2017–2022 (row (3)), $`\hat{\beta}`$ stays significant, while the coefficients of the two channels keep their sign but lose precision.

Dropping one sector at a time keeps $`\hat{\beta}`$ between −0.196 and −0.150 and all three estimates, $`\hat{\beta}`$, $`\hat{\beta}^{f}`$ and $`\hat{\beta}^{e}`$, negative and significant at the 1% level (Figure OA1). Without the 22 manufacturing sectors, $`\hat{\beta}`$ is similar but imprecise.

Two further checks concern the instrument and the two-channel equation. With one of the 27 products dropped from the instrument at a time, our headline estimate ranges from −0.171 to −0.151, with a first-stage $`F`$ of at least 36. After the sector and year effects, the dollar price term and the real exchange rate term of eq. (20) have a correlation of −0.56, so they are not collinear.

<a name="table-oa2"></a>**Table OA2. Real interest rate control and long difference**

|                                        | Eq.&nbsp;(19)<br>$`\beta`$ | Eq.&nbsp;(19)<br>$`F`$ | Eq.&nbsp;(20)<br>$`\beta^{f}`$ | Eq.&nbsp;(20)<br>$`\beta^{e}`$ | $`N/G`$ |
|:---------------------------------------|:--------------------------:|:----------------------:|:------------------------------:|:------------------------------:|:-------:|
| (1) Baseline                           | −0.159<sup>\*\*\*</sup>    | 352                    | −0.184<sup>\*\*\*</sup>        | −0.212<sup>\*\*\*</sup>        | 719/63  |
|                                        | (0.027) [0.006]            |                        | (0.031) [0.005]                | (0.056) [0.015]                |         |
| (2) $`m_{j}\times`$ real interest rate | −0.168<sup>\*\*\*</sup>    | 84                     | −0.161<sup>\*\*\*</sup>        | −0.188<sup>\*\*\*</sup>        | 719/63  |
|                                        | (0.048) [0.026]            |                        | (0.031) [0.006]                | (0.059) [0.044]                |         |
| (3) Long difference, 2017–2022         | −0.121<sup>\*\*\*</sup>    | 80                     | −0.128                         | −0.343                         | 56/56   |
|                                        | (0.035) [0.005]            |                        | (0.087) [0.122]                | (0.274) [0.241]                |         |

Notes: 2SLS estimates of eqs. (19) and (20). Row (1) is column (1) of Tables 2 and 3. Row (2) adds $`m_{j}`$ times the real interest rate, the commercial loan rate less expected inflation. Row (3) uses the changes over 2017–2022, one observation per sector, with a constant. $`F`$: cluster-robust first-stage $`F`$ of $`\beta`$. Homogeneity: with $`m_{j}\ln P_{m}`$ and $`m_{j}\ln w`$ as separate regressors, both instrumented by the current and the lagged instrument, the coefficients are −0.321 and 0.366, and their sum, 0.045 (0.022), is significant at the 5% level, so homogeneity holds only approximately. Standard errors clustered by sector in parentheses; stars and brackets as in Table 2.

<a name="figure-oa1"></a>![Figure OA1. Estimates without one sector at a time](figures/fig_loo.png)

**Figure OA1. Estimates without one sector at a time**

Notes: Each row drops the sector named on the left: (a) $`\beta`$ of eq. (19); (b) $`\beta^{f}`$ and (c) $`\beta^{e}`$ of eq. (20). Markers: estimates; lines: 95% intervals, clustered by sector; vertical line: the estimate on all 63 sectors.

## OA.4 Inference

In the placebo draws of Table B2, the clustered test at the 5% level rejects in 48% of the draws for 2SLS and in 59% for the reduced form, so clustered standard errors over-reject. The wild cluster bootstrap also over-rejects, but less: it rejects in 22% of the draws for the reduced form.

## OA.5 Supplier prices

Table OA3 gives the cumulative responses by route for months 0 to 3 and 12. With all 21 products (Panel A), the network response ($`\phi_{n}`$) builds up over the year while the direct response ($`\phi_{d}`$) fades. Without electricity and gas (Panel B), the network response stops building up after the first month, so the build-up in Table 4 comes mostly from electricity and gas. The agricultural and service products added in Panel B of Table 4 are priced by the agricultural and services PPI.

<a name="table-oa3"></a>**Table OA3. Cumulative supplier price responses, with and without electricity and gas**

|                                                             | Month 0                | Month 1                | Month 2                | Month 3                | Month 12            |
|:------------------------------------------------------------|:----------------------:|:----------------------:|:----------------------:|:----------------------:|:-------------------:|
| **Panel A: 21 supplier products**                           |                        |                        |                        |                        |                     |
| Direct, $`\phi_{d}`$                                        | 1.118<sup>\*\*\*</sup> | 1.207<sup>\*\*\*</sup> | 1.261<sup>\*\*\*</sup> | 1.294<sup>\*\*\*</sup> | 0.179               |
|                                                             | (0.127)                | (0.189)                | (0.266)                | (0.377)                | (0.452)             |
| Network, $`\phi_{n}`$                                       | 1.358<sup>\*\*\*</sup> | 1.755<sup>\*\*\*</sup> | 2.600<sup>\*\*\*</sup> | 2.313<sup>\*</sup>     | 3.754<sup>\*</sup>  |
|                                                             | (0.336)                | (0.538)                | (0.941)                | (1.329)                | (2.212)             |
| **Panel B: Without electricity and gas (D35), 20 products** |                        |                        |                        |                        |                     |
| Direct, $`\phi_{d}`$                                        | 1.134<sup>\*\*\*</sup> | 1.198<sup>\*\*\*</sup> | 1.068<sup>\*\*\*</sup> | 1.007<sup>\*\*\*</sup> | −0.344<sup>\*</sup> |
|                                                             | (0.165)                | (0.235)                | (0.221)                | (0.241)                | (0.193)             |
| Network, $`\phi_{n}`$                                       | 1.518<sup>\*</sup>     | 1.666                  | 0.759                  | −0.410                 | −1.216<sup>\*</sup> |
|                                                             | (0.846)                | (1.135)                | (0.926)                | (1.079)                | (0.681)             |

Notes: Cumulative coefficients of eq. (25), split by route, with twelve monthly lags and product and month effects, 2013M1–2024M12; 3,024 product-months in Panel A and 2,880 in Panel B. Months 2 and 12 of Panel A are columns (4) and (6) of Table 4; month 0 differs from column (2), which has no lags. Standard errors clustered by product in parentheses; stars as in Table 2.

## OA.6 The lagged coefficient of Table 5

Table OA4 splits the coefficients of column (3) of Table 5 into parts that add up exactly, on the sector-years with positive published value added. The partial recovery in the following year comes mostly from the stock term and from personnel costs catching up, two thirds of the catch-up through wages. With value added as published, the lagged coefficient is small and not significant.

<a name="table-oa4"></a>**Table OA4. The coefficients of Table 5, column (3), by component**

|                                                                 | Year of the change, $`\beta_{0}`$ | Following year, $`\beta_{1}`$ | Two-year sum            |
|:----------------------------------------------------------------|:---------------------------------:|:-----------------------------:|:-----------------------:|
| (1) Labor share, $`\ln s_{L}`$                                  | −0.257<sup>\*\*\*</sup>           | 0.111<sup>\*\*</sup>          | −0.146<sup>\*\*\*</sup> |
|                                                                 | (0.031)                           | (0.045)                       | (0.039)                 |
| (2) Stock term, $`\ln(VA^{pub}/VA)`$                            | −0.095<sup>\*\*</sup>             | 0.062<sup>\*\*\*</sup>        | −0.033                  |
|                                                                 | (0.038)                           | (0.016)                       | (0.038)                 |
| (3) Labor share with published value added, $`\ln s^{pub}_{L}`$ | −0.162<sup>\*\*\*</sup>           | 0.049                         | −0.113<sup>\*\*\*</sup> |
|                                                                 | (0.051)                           | (0.051)                       | (0.039)                 |
| (4) &emsp;Personnel costs, $`\ln W`$                            | 0.009                             | 0.042<sup>\*\*</sup>          | 0.051                   |
|                                                                 | (0.028)                           | (0.018)                       | (0.039)                 |
| (5) &emsp;&emsp;Wage, $`\ln w`$                                 | 0.011                             | 0.028<sup>\*</sup>            | 0.039<sup>\*</sup>      |
|                                                                 | (0.011)                           | (0.015)                       | (0.021)                 |
| (6) &emsp;&emsp;Employment, $`\ln L`$                           | −0.002                            | 0.014                         | 0.012                   |
|                                                                 | (0.024)                           | (0.012)                       | (0.033)                 |
| (7) &emsp;Published value added, $`-\ln VA^{pub}`$              | −0.171<sup>\*\*\*</sup>           | 0.007                         | −0.164<sup>\*\*\*</sup> |
|                                                                 | (0.060)                           | (0.061)                       | (0.060)                 |

Notes: 2SLS estimates of eq. (26), as in column (3) of Table 5, with each component as the dependent variable, on the 643 sector-years of 2014–2024 with positive published value added; Sanderson–Windmeijer $`F`$ 135 and 293 for the current and the lagged regressor. Rows (1) = (2) + (3), (3) = (4) + (7) and (4) = (5) + (6). On all 651 sector-years the lagged coefficient is 0.113 (Table 5). Standard errors clustered by sector in parentheses; stars as in Table 2.

## OA.7 Local projections

Local projections (Jordà, 2005) estimate the response of the labor share at each horizon separately. For $`h=0,\ldots,3`$,

```math
\ln s_{L,j,t+h}-\ln s_{L,j,t-1}=\beta_{h}\,m_{j}\ln\left(\frac{P_{m,jt}}{C_{jt}}\right)+\gamma_{h}\,m_{j}\ln\left(\frac{P_{m,j,t-1}}{C_{j,t-1}}\right)+\delta^{h}_{j}+\delta^{h}_{t}+\varepsilon_{j,t+h}, \qquad \text{(OA.1)}
```

where $`C_{jt}`$ is the wage and $`\delta^{h}_{j}`$ and $`\delta^{h}_{t}`$ are sector and year effects. The second regressor holds the previous year’s price fixed, so $`\beta_{h}`$ is the response to a rise in year $`t`$, and both regressors are instrumented by $`m_{j}Z^{f}`$ of the same year.

In the year of the rise the labor share falls about as much as the static estimate on the same observations implies (Table OA5), and the response one year later is imprecise. Two years later materials are cheaper relative to the wage than before the rise, and the labor share is above its initial level. Averaged over the next three years, the response per unit of the price change does not differ significantly from the response on impact, so there is no delayed effect beyond the year of the change. In sectors with a larger rise the labor share was already falling the year before, but controlling for this lagged change leaves the pattern unchanged (last row).

<a name="table-oa5"></a>**Table OA5. Local projections of the labor share**

|                                           | $`\ln s_{L,jt}`$<br>(1) Static | $`\ln s_{L,j,t+h}`$<br>$`-\ln s_{L,j,t-1}`$<br>(2) $`h=0`$ | $`\ln s_{L,j,t+h}`$<br>$`-\ln s_{L,j,t-1}`$<br>(3) $`h=1`$ | $`\ln s_{L,j,t+h}`$<br>$`-\ln s_{L,j,t-1}`$<br>(4) $`h=2`$ | $`\ln s_{L,j,t+h}`$<br>$`-\ln s_{L,j,t-1}`$<br>(5) $`h=3`$ |
|:------------------------------------------|:------------------------------:|:----------------------------------------------------------:|:----------------------------------------------------------:|:----------------------------------------------------------:|:----------------------------------------------------------:|
| $`m_{j}\ln(P_{m,jt}/w_{jt})`$             | −0.208<sup>\*\*\*</sup>        | −0.205<sup>\*\*\*</sup>                                    | −0.031                                                     | 0.283<sup>\*\*\*</sup>                                     | 0.159<sup>\*\*\*</sup>                                     |
|                                           | (0.035) [0.024]                | (0.038) [0.030]                                            | (0.073) [0.715]                                            | (0.035) [0.006]                                            | (0.040) [0.115]                                            |
| Static prediction                         |                                | −0.208                                                     | −0.285                                                     | 0.108                                                      | 0.163                                                      |
| Path of $`m_{j}\ln(P_{m}/w)`$             |                                | 1                                                          | 1.373<sup>\*\*\*</sup>                                     | −0.520<sup>\*\*\*</sup>                                    | −0.786<sup>\*\*\*</sup>                                    |
|                                           |                                |                                                            | (0.147)                                                    | (0.142)                                                    | (0.130)                                                    |
| Controlling for $`\Delta\ln s_{L,j,t-1}`$ |                                | −0.258<sup>\*\*\*</sup>                                    | −0.125<sup>\*</sup>                                        | 0.175<sup>\*\*\*</sup>                                     | 0.055                                                      |
|                                           |                                | (0.047) [0.024]                                            | (0.064) [0.069]                                            | (0.027) [0.014]                                            | (0.039) [0.327]                                            |

Notes: Column (1): eq. (19) on the observations of columns (2)–(5). Columns (2)–(5): eq. (OA.1) with start years 2014–2021 and the same 447 observations of 59 sectors at every horizon (442 with the control). First-stage $`F`$ of Sanderson and Windmeijer (2016): 355 and 129 (398 and 138 with the control), 494 in column (1). Path: the response of $`m_{j}\ln(P_{m,jt}/w_{jt})`$ itself; static prediction: column (1) times the path. Per unit of the path, the response averages −0.256 over $`h=1`$ to 3, against −0.205 at $`h=0`$; the difference, −0.051 (0.055), is not significant. With $`\ln s_{L,j,t-2}-\ln s_{L,j,t-1}`$ on the left, the coefficient is 0.175 (0.038). Standard errors clustered by sector in parentheses; stars and brackets as in Table 2.

## OA.8 Heterogeneity and the share equation

Table OA6 interacts the regressor with the markup itself rather than with its terciles (Table 6, Panel B). The interaction is negative, as (P2) predicts, but imprecise. In Panel C of Table 6, the standard error of $`\beta^{implied}`$ comes from the delta method with $`\hat{\sigma}`$ and $`\bar{\mu}`$ independent, and its test against $`\hat{\beta}`$ treats the two estimates as independent.

<a name="table-oa6"></a>**Table OA6. Markup interaction**

|                                            | 2SLS                  |
|:-------------------------------------------|:---------------------:|
| $`m_{j}\ln(P_{m}/w)`$                      | −0.206<sup>\*\*</sup> |
|                                            | (0.102) [0.125]       |
| $`(\mu_{j}-\bar{\mu})\,m_{j}\ln(P_{m}/w)`$ | −0.423                |
|                                            | (0.906) [0.778]       |
| Smallest SW $`F`$                          | 161                   |
| $`N/G`$                                    | 713/62                |

Notes: 2SLS estimate of eq. (19) with the regressor and the instrument also interacted with the 2009–2012 markup, centered at its mean of 1.196. SW $`F`$: Sanderson–Windmeijer. Standard errors clustered by sector in parentheses; stars and brackets as in Table 2.

## OA.9 Contributions to the labor share

In 2017–2022 the labor share of the 53 sectors of Table 7 fell from 44.86% to 30.54%, most of the fall within sectors, and the year effects of eq. (19), which the contributions leave out, fell by 0.179 log points. The 95% interval of the two-channel total over these years is [−4.75, −1.58] pp. Split by the shocks themselves, in the reduced form with $`m_{j}Z^{f}_{jt}`$ in place of the dollar price term, higher world prices lowered the labor share by 2.20 pp and the real depreciation by 1.54 pp. This split need not add up to the two-channel total, since the dollar price of materials also moves with domestic shocks.

Sector contributions from eq. (28) are converted into pp with the previous-year labor share, weighted by previous-year value added and summed over the years of a period. For the national accounts labor share, they are averaged within sections with previous-year personnel costs as weights and converted with section value added and labor shares; they are zero for sections A, D, P, Q and R.

## References

Gürkaynak, R. S., Kısacıkoğlu, B. and Lee, S. S. (2023). Exchange rate and inflation under weak monetary policy: Turkey verifies theory. *Economic Policy*, 38(115), 519–560. https://doi.org/10.1093/epolic/eiad020

Jordà, Ò. (2005). Estimation and inference of impulse responses by local projections. *American Economic Review*, 95(1), 161–182. https://doi.org/10.1257/0002828053828518

Pierce, J. R. and Schott, P. K. (2012). A concordance between ten-digit U.S. Harmonized System codes and SIC/NAICS product classes and industries. *Journal of Economic and Social Measurement*, 37(1–2), 61–96. https://doi.org/10.3233/JEM-2012-0351

Sanderson, E. and Windmeijer, F. (2016). A weak instrument F-test in linear IV models with multiple endogenous variables. *Journal of Econometrics*, 190(2), 212–221. https://doi.org/10.1016/j.jeconom.2015.06.004
