# coxrt - Cox Regression for Right Truncated Data

The  `coxrt` package fits Cox regression based on retrospectively ascertained time-to-event
data. The method uses Inverse-Probability-Weighting (IPW) estimating equations with stabilized weights as described
in B. Vakulenko-Lagun, M. Mandel, and R. A. Betensky, 2018, 
“Inverse-Probability-Weighting Methods for Cox Regression with Right Truncated Data” (submitted to Biometrics).

The `coxrt` package provides two functions: `coxph.RT` that assumes positivity and
`coxph.RT.a0` that allows for adjustment of estimation under violation of positivity. The
illustrative examples in these functions include analysis of AIDS latency data with age as a
covariate, where the AIDS cases were retrospectively ascertained at June 30, 1986, and only
those who developed AIDS by that time were included in the analysis (Kalbfeisch and Lawless,
1989). For examples we refer to the package vignette:
```{r}
rmarkdown::render("vignettes/coxrt-vignette.Rmd")
```
The  `coxrt` package can be installed by
```{r}
devtools::install_github(“Bella2001/coxrt”)
```
 
 
 
 
