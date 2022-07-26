Example of `pipreq` on Jupyter Notebook:
```shell
pipreqsnb --savepath ./a3/python3.8.10_requirements.txt ./a3/a3.ipynb
```
# Questions
- What is the difference between Shapiro-Wilk and Z-test? Both test for normality.
- A1. qqplot: How to add `ci_mean` (like in statsmodels) confidence interval?
- Why are Shapiro–Wilk W-statistic, t-statistic, F-statistic (when not 1) or Z-statistic shown, but we cannot use them directly? How `p-values` are calculated for these statistics?
- A3.1.4 fit4 and fit5: How to do orthogonal polynomials? Do I have the correct implementation? Which algorithm is used in R and how can it be reproduced in Python (with numpy, preferably)?
- A3. beat: How to use `seaborn.pairplot()` as `matplotlib` subplot (usually by supplying `ax` parameter)?
- A4.1.2.2: How to change the sign of the coefficients? Is it because of the order of values? Should it be fixed through contrasts' matrix encoding using `C(Direction, contrast)`?
- A4.1.2.4: How to use the R-like formula? There is no integration of `sklearn` with `patsy`.
- A4.1.2.8: How to set random seed in `sklearn` for `KNeighborsClassifier`? I can only do `np.random.seed(1)`, but I do not think it is related.
- A6 `Check the importance`: How can I get `IncNodePurity` (increment in node purity) from `sklearn.ensemble.RandomForestRegressor`? I couldn’t find a way to get aggregated node purity increase.

# Assignment Typos
- "Interprete" instead of "Interpret" in all places;
- A6 `ggscatter(Carseats, x = "Sales", y = "Price" ...`: axis labels were switched;
- A6.1.2.4 `when building a random forest of classification trees`: _regression_ tees are meant because `medv` in `Boston` is of float type;

# TODO:
- experiment to understand better A7.`plot_svm`;
