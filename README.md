Example of `pipreq` on Jupyter Notebook:
```shell
pipreqsnb --savepath ./a3/python3.8.10_requirements.txt ./a3/a3.ipynb
```
# Questions
- What is the difference between Shapiro-Wilk and Z-test? Both test for normality.
- A1.qqplot: Add `ci_mean` (like in statsmodels) confidence interval.
- Why Shapiro–Wilk W-statistic, t-statistic, F-statistic (when not 1) or Z-statistic is shown, but we cannot use them directly? How `p-values` are calculated for these statistics?
- What about intermediate values in ANOVA (except `p-values` and SSR in comparison)?
- A3.1.4.fit4+: How to do orthogonal polynomials? Which algorithm is used in R and how can it be reproduced in Python (with numpy, preferably)? My model has similar metrics and other coefficients, so my guess is that I failed to put the constant coefficients for the orthogonal polynomial terms.
- A3.beat: How to use `seaborn.pairplot()` as `matplotlib` subplot.
- A4.1.2.2: How to change the sign of the coefficients? Is it because of order of values? Should it be fixed through contrasts' matrix encoding using `C(Direction, contrast)`?
- A4.1.2.4: How to use R-like formula? There is no integration of `sklearn` with `patsy`.
- A4.1.2.8: How to set random seed in `sklearn` for `KNeighborsClassifier`? I can only do `np.random.seed(1)`, but I do not know if it is related.

# Bugs
- A6. `ggscatter(Carseats, x = "Sales", y = "Price" ...` - axis labels were switched;
