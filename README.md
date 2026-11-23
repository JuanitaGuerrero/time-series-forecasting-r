# Time Series Forecasting and Ecological Cycles in R

Time-series analysis, forecasting, and frequency-domain methods applied to public-health-related and ecological examples. Developed as part of a Quantitative Biology workshop at Universidad de los Andes.

## Analyses

**Corticosteroid subsidies:** monthly Australian corticosteroid subsidy series (`h02` from `fpp2`), STL decomposition, seasonal plots, residual autocorrelation, comparison of ARIMA, ETS, seasonal regression (TSLM), seasonal naive, random walk with drift, and mean benchmarks. The workshop also holds out the final 24 months for forecast assessment (RMSE).

**Hare–lynx cycles:** the `pelt` time series, periodogram and dominant cycle estimation, cross-correlation, and wavelet coherence to explore time-varying synchronization between hare and lynx populations.

## Repository contents

- `analysis/workshop-07-time-series.Rmd`: R Markdown analysis and interpretation (Spanish)
- `README.md`: overview and reproducibility notes (English)

The analyses use datasets included with R packages; no separate CSV files were supplied or required by the source document.

## Requirements

R packages: `fpp2`, `fpp3`, `tidyverse`, `biwavelet`; plus an R Markdown environment with XeLaTeX to render the original PDF output.

```r
install.packages(c("fpp2", "fpp3", "tidyverse", "biwavelet", "rmarkdown"))
```

Open `analysis/workshop-07-time-series.Rmd` in RStudio and knit to PDF. Package versions may affect results. **The code has not been executed or independently validated in this repository.**

## Authorship

Code and analyses: **Juanita Guerrero**. The repository version updates the cover-page attribution at the author's request; the original academic submission listed a group partner. This is a course-work demonstration rather than a peer-reviewed research publication.
