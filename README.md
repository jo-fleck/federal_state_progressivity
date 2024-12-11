## Estimates of U.S. Federal and State Fiscal Progressivity

The estimates in the folders are from the paper "Fiscal Progressivity of the U.S. Federal and State Governments" (J. Fleck, J. Heathcote, K. Storesletten, G. Violante; December 2024).

Please cite the paper when using the estimates.

### Readme (see Appendix O)

For each of our sample year pairs (2005/06, 2010/11 and 2015/16), the spreadsheets on this webpage contain five sets of progressivity estimates for our baseline tax and transfer specification (see Sections 3 and 4). The estimates differ regarding the sorts of taxes and transfers included in household disposable income:

1. **agg_state**: includes state and local taxes and transfers
2. **federal**: includes federal taxes and transfers
3. **federal_agg_state**: includes federal, state and local taxes and transfers
4. **state**: includes state and local taxes and transfers
5. **state_federal**: includes federal, state and local taxes and transfers

Estimates 1, 2, and 3 provide aggregate U.S. progressivity estimates and are constructed using the original ASEC household weights. Estimates 4 and 5 provide state-level progressivity estimates for each U.S. state and the District of Columbia, and are based on adjusted ASEC household weights (see Appendix I).

The files in turn contain three sets of parameter estimates, corresponding to the following three models:
- HSV estimated by OLS
- HSV estimated by PPML
- HSV-T estimated by non-linear least squares

Note that the parameter $\tau$ is independent of the scale of the economy. In contrast, the parameter $\lambda$ and the parameter $Tr$ in the HSV-T specification do depend on the scale. We therefore report two values for $\lambda$. One is the $\lambda$ estimated using nominal current dollar values for pre and post-government income. The second $\lambda$ value reported for each state $s$ is $\hat{\lambda}_s = \lambda_s \times Y_s^{-\tau_s}$ where $Y_s$ is average state household pre-government income. This $\hat{\lambda}_s$ is interpretable as the $\lambda_s$ value that one would estimate if both pre- and post-government income are expressed relative to average state pre-government income. In particular 

$$\frac{\tilde{y}}{Y_s} = \lambda_s Y_s^{-\tau_s} \left(\frac{y}{Y_s}\right)^{1-\tau_s} = \hat{\lambda}_s \left(\frac{y}{Y_s}\right)^{1-\tau_s}$$

Users of our estimates should either (i) scale model variables so that mean pre-government income is equal to one and set $\lambda_s = \hat{\lambda}_s$, or (ii) compute mean pre-government income $\bar{Y}_s$ in their data and set $\lambda_s = \hat{\lambda}_s \times \bar{Y}_s^{\tau_s}$. We similarly report two $Tr$ values: $Tr_s$, which corresponds to an estimate of nominal current dollar lump-sum transfers in state $s,$ and $\widehat{Tr}_s=Tr_s/Y_s$, which corresponds to lump-sum transfers as a share of mean state household pre-government income.
