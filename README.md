# Bitcoin Multiple Regression Inference
-  To infer which features are massively associated with bitcoin price, what kind of relationship they have with it, and whether this relationship is simple or more complex with interaction/ploynomial features.¶
-  Data collected from [**Yahoo Finance**](https://uk.finance.yahoo.com/), [**Google Trends**](https://trends.google.com/trends) and [**Blockchain.com**](https://www.blockchain.com/) using relevant APIs and pickled for further analysis.
- Performed **eploratory data analysis** to narrow down dataframe, and did appopriate **model diagnostics** to check if linear model assumptions hold and observe **outliers and high leverage points**.
- Checked for **autocorrelation** to confirm the data points are indepedent and not highly correlated with a lag of 1 day.
- Performed **multiple regression modelling with statsmodel** initially, then with **scikit-learn** after checking for **polynomial/interaction affects**.
- Used model **shrinkage methods, stepwise regression and best subset selection** to counter **multicollinearity** between predictors and select the most significant features.
- Found out that apart from **total market capitalization of bitcoin**, which obviously is a function of bitcoin price, the **interest index** by google trends and **daily number of total transactions** of bitcoin highly affect its price.
- It was also inferred that **bitcoin valuation is more affected by tech stocks valuation** especifically the **NASDAQ-100** index compared to the **S&P-500** index.

![](https://github.com/harrisasadb/Bitcoin-Multiple-Regression-Inference/blob/main/bitcoin%20pics/correlation.png)
![](https://github.com/harrisasadb/Bitcoin-Multiple-Regression-Inference/blob/main/bitcoin%20pics/plot.png)
![](https://github.com/harrisasadb/Bitcoin-Multiple-Regression-Inference/blob/main/bitcoin%20pics/interest.png)
![](https://github.com/harrisasadb/Bitcoin-Multiple-Regression-Inference/blob/main/bitcoin%20pics/residual.jpg)
![](https://github.com/harrisasadb/Bitcoin-Multiple-Regression-Inference/blob/main/bitcoin%20pics/subset.jpg)

