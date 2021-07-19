# RGAP: R Package for Production Function Output Gap Estimation

RGAP provides tools for modeling and estimating the bivariate unobserved component models involved in the Cobb-Douglas production function methodology to estimate the output gap.

[KOF Working Paper](https://kof.ethz.ch/publikationen/kof-working-papers.html)

If you use RGAP in your paper, please cite it properly, see `citation("RGAP")` in R, or above link to the paper.

## Details

The output gap indicates the percentage difference between the actual output of an economy and its potential. Since potential output is a latent process, the estimation of the output gap poses a challenge and numerous filtering techniques have been proposed. RGAP facilitates the estimation of a Cobb-Douglas production function type output gap, as suggested by the European Commission (Havik et al. 2014). To that end, the non-accelerating wage rate of unemployment (NAWRU) and the trend of total factor productivity (TFP) can be estimated in two bivariate unobserved component (UC) models by means of Kalman filtering and smoothing. RGAP features a flexible modeling framework for the appropriate state-space models and offers frequentist as well as Bayesian estimation techniques.

## Main features

- Data fetching from AMECO database
- Data pre processing
- Modeling bivariate state-space models for the NARWU and the TFP trend
- Estimation of defined models via the Kalman filter and smoother and
  - maximum likelihood estimation or
  - bayesian estimation via Gibbs procedure
- Output gap computation
- Alternative approaches: HP-filter and bivariate UC model by Kuttner (1994)

## Install the package
Since the package is not on CRAN just yet, you can install it using the **install_github** function from the **devtools** package.
``` 
library(devtools)
install_github('sinast3000/RGAP')
```

***

Kuttner, K. N. (1994), Estimating potential output as a latent variable, Journal of Business & Economic Statistics 12(3), 361–368.

Havik, K., Mc Morrow, K., Orlandi, F., Planas, C., Raciborski, R., R¨oger, W., Rossi, A., Thum-Thysen, A. & Vandermeulen, V. (2014), The production function methodology for calculating potential growth rates & output gaps, Technical report, Directorate
General Economic and Financial Affairs (DG ECFIN), European Commission.

