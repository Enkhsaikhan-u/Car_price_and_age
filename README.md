# Mini project: Car price and age 

**Author:** Enkhsaikhan Usny-Ekh  


## 📖 Description

This mini project explores the relationship between car price and age for used cars in Chicago and Los Angeles. This analysis finds a negative association: the price is lower, on average, by 11.3% for every additional year of age. 

## 📊  Data Sources

Data is taken from the case study of textbook *Data Analysis for Business, Economics and Policy by Gabor Bekes and Gabor Kezdi.*

## 📂 Folder Structure
- `data/` – Raw datasets  
- `code/` – Python scripts  
- `output/` = Graphs and tables made through the analysis     
- `README.md` – Project documentation  


## ⚙️ Computational Requirements

This project uses Python 3.10+ and requires several data analysis libraries. 

The following packages are required to run the analysis
- numpy
- pandas
- matplotlib
- seaborn
- statmodels
- scipy

Example installation:
```python
pip install pandas numpy statsmodels matplotlib seaborn scipy
```

## 📈 Results

### OLS Regression Results
|                          |                             |
|---------------------------|-----------------------------|
| **Dep. Variable:**        | lprice                      |
| **Model:**                | OLS                         |
| **Method:**               | Least Squares               |
| **Date:**                 | Sat, 04 Oct 2025            |
| **Time:**                 | 20:03:15                    |
| **No. Observations:**     | 548                         |
| **Df Residuals:**         | 546                         |
| **Df Model:**             | 1                           |
| **R-squared:**            | 0.430                       |
| **Adj. R-squared:**       | 0.429                       |
| **F-statistic:**          | 433.5                       |
| **Prob (F-statistic):**   | 2.62e-71                    |
| **Log-Likelihood:**       | -628.56                     |
| **AIC:**                  | 1261.                       |
| **BIC:**                  | 1270.                       |
| **Covariance Type:**      | HC1                         |

#### Coefficients
| Variable   | Coef.   | Std. Err. | z       | P>|z| | [0.025 | 0.975] |
|-------------|----------|-----------|---------|------|---------|---------|
| Intercept  | 9.6637   | 0.077     | 125.363 | 0.000 | 9.513  | 9.815  |
| age        | -0.1125  | 0.005     | -20.821 | 0.000 | -0.123 | -0.102 |

#### Model Diagnostics
|                      |         |
|----------------------|---------|
| **Omnibus:**         | 640.126 |
| **Prob(Omnibus):**   | 0.000   |
| **Jarque-Bera (JB):**| 54797.694 |
| **Prob(JB):**        | 0.000   |
| **Skew:**            | -5.518  |
| **Kurtosis:**        | 50.730  |
| **Durbin-Watson:**   | 2.035   |
| **Cond. No.:**       | 31.2    |

**Notes:**  
[1] Standard errors are heteroscedasticity robust (HC1).


## 🖼️ Diagram
![Model Flow](../output/scatter.png)

