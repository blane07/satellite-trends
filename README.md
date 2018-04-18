# Satellite Trends [![MIT license](http://img.shields.io/badge/license-MIT-brightgreen.svg)](http://opensource.org/licenses/MIT)

#### Why?
To gain a better understanding of today's satellite market

#### How?
Exploring data of current operational satellites

#### Data
The Union of Concerned Scientists (UCS) provided the dataset. It's free and available to the public at: https://www.ucsusa.org/nuclear-weapons/space-weapons/satellite-database#.Wtdob3UbOfg

#### Findings

![Nano Satellite Trends](https://github.com/blane07/satellite-trends/blob/master/images/nano_sat_trend.png)
* The number of operational nanosatellites grows at an exponential rate

* The model's results are below. It's a ordinary least squares (linear) regression of **Launch Year** and the *logarthim* of **The Number of Operational Satellites**
```
                            OLS Regression Results                            
==============================================================================
Dep. Variable:                      y   R-squared:                       0.861
Model:                            OLS   Adj. R-squared:                  0.843
Method:                 Least Squares   F-statistic:                     49.37
Date:                Sun, 11 Mar 2018   Prob (F-statistic):           0.000110
Time:                        10:18:50   Log-Likelihood:                -8.1042
No. Observations:                  10   AIC:                             20.21
Df Residuals:                       8   BIC:                             20.81
Df Model:                           1                                         
Covariance Type:            nonrobust                                         
==============================================================================
                 coef    std err          t      P>|t|      [0.025      0.975]
------------------------------------------------------------------------------
const       -944.5638    134.800     -7.007      0.000   -1255.412    -633.715
x1             0.4707      0.067      7.027      0.000       0.316       0.625
==============================================================================
Omnibus:                        2.684   Durbin-Watson:                   1.104
Prob(Omnibus):                  0.261   Jarque-Bera (JB):                0.823
Skew:                          -0.694   Prob(JB):                        0.663
Kurtosis:                       3.218   Cond. No.                     1.41e+06
==============================================================================
```

#### More
* Please refere to [**operational-satellites.ipynb**](https://github.com/blane07/satellite-trends/blob/master/operational-satellites.ipynb)
