# NETFLIX SHARE PRICE ANALYSIS
 - In this analytical report, we delve into Netflix's stock prices, utilizing a
comprehensive dataset spanning from 2023 to 2024. This introductory section provides a brief
overview of the dataset, its source, contents, and outlines the analytical approach employed for
the exploratory data analysis (EDA)

## **Source of Data**
- The data was sourced from Yahoo Finance using the pandas data reader library in Python, ensuring accuracy and reliability in representing Netflix's stock performance.
- 
## **Contents of Data**
  - Encompassing various facets of Netflix's stock market journey, the dataset comprises essential
columns elucidating crucial aspects of stock pricing. These include:
- Date: Recording the trading days over the specified time frame.
- Open: Signifying the opening price of Netflix stock on each trading day.
- High: Reflecting the highest price at which Netflix stock traded during the day.
- Low: Denoting the lowest price at which Netflix stock traded during the day.
- Close: Indicating the closing price of Netflix stock on each trading day.
- Adjustment Close: Presenting the adjusted closing price, accounting for events such as
 dividends and stock splits.
- Volume: Representing the total number of shares traded on each trading day
- 
 ## **Analytical Approach**
  
 -  The analytical approach adopted for this analysis primarily revolves around Exploratory Data
Analysis (EDA). Through rigorous examination and visualization of the dataset, we aim to
unearth insightful patterns, trends, and relationships within Netflix's stock prices. By
scrutinizing the data from multiple angles,  to extract actionable insights that can
inform strategic decision-making and deepen our understanding of the dynamics influencing
Netflix's stock performance.

**Overview of The Data**

    - Reading and understanding the data.
    
**Data Cleaning**

    - Data cleaning involves identifying and rectifying errors, inconsistencies, and missing values within a dataset to ensure its accuracy and reliability. This process includes removing duplicate entries, handling missing data, standardizing data formats, addressing outliers, and correcting any inconsistencies. By cleaning the data, we ensure that our analysis is based on accurate and reliable information, enabling us to draw meaningful insights and make informed decisions.
 ## Time Series Analysis
 - Time series analysis is a powerful statistical technique used to analyze and interpret data points
collected at successive intervals of time. Unlike traditional cross-sectional data analysis, which
focuses on observations at a single point in time, time series analysis delves into the temporal
patterns, trends, and dependencies present in the data. It finds applications across various
domains, including finance, economics, meteorology, and engineering, where understanding the
behavior of a phenomenon over time is crucial for decision-making and prediction. Time series
data often exhibits unique characteristics such as trend, seasonality, autocorrelation, and
volatility, which necessitate specialized analytical techniques for exploration and forecasting.
Through time series analysis, practitioners can uncover valuable insights, detect anomalies,
model relationships, and make informed predictions about future outcomes, thereby enabling
proactive decision-making and strategic planning. This introductory paragraph sets the stage for
a deeper dive into the methods and tools used in time series analysis, empowering analysts to
extract meaningful insights and derive actionable conclusions from temporal data.

## Time Series Visualization
- Upon examining the side-by-side comparison of the "Open" and "Close" time series plots, it
becomes evident that the patterns exhibited by both columns are strikingly similar. However,
subtle differences can be observed between the two. In the "Open" plot, the price initiates with a
slight uptick at the beginning of the trading day, indicating an initial surge in market activity.
Conversely, in the "Close" plot, the price experiences a marginal decline towards the end of the
trading day, reflecting a potential decrease in market sentiment as trading comes to a close.
Despite these minor discrepancies, the overarching trends and fluctuations in both plots align closely, suggesting a strong correlation between the opening and closing prices of the Netflix
stock over the analyzed time period.
##  Descriptive Statistics
- Description of Insights:
• The correlation matrix reveals the correlation coefficients between the "Open", "High",
"Low", and "Close" prices of Netflix shares.
• A correlation coefficient ranges from -1 to 1, where 1 indicates a perfect positive linear
relationship, -1 indicates a perfect negative linear relationship, and 0 indicates no linear
relationship.
• In this correlation matrix:
– The diagonal elements represent the correlation of each variable with itself,
which is always 1.
– Off-diagonal elements represent the correlations between pairs of variables.
• The correlation coefficients close to 1 suggest a strong positive linear relationship
between the corresponding pairs of variables.
• Specifically:
– The "Open" price is highly correlated with the "High", "Low", and "Close" prices,
with correlation coefficients of approximately 1.
– Similarly, the "High", "Low", and "Close" prices exhibit strong positive
correlations among themselves, all close to 1.
• The high correlations between these variables indicate that they move in tandem, which
is typical in financial time series data where the opening, high, low, and closing prices are
closely related.

##  Correlation Matrix
 Highest and Lowest Share Prices
6. Seasonality in Stock Prices
## Predictive Analysis
**Model Prediction**:
  Model prediction plays a pivotal role in forecasting the future
trajectory of stock prices. Leveraging advanced statistical techniques, analysts can develop
models that harness historical data to make informed predictions about future price
movements. These predictions serve as valuable insights for investors, guiding their decisionmaking processes and informing strategic investment choices.

**Potential Outcome of Predictions**:
The outcomes of prediction hold significant implications for investors and stakeholders in the
financial market. Accurate predictions enable investors to anticipate market trends, identify
profitable investment opportunities, and mitigate risks associated with market volatility.
Conversely, inaccurate predictions can lead to suboptimal investment decisions, resulting in
financial losses and missed opportunities. Therefore, the reliability and precision of prediction
models are paramount for enhancing investment performance and maximizing returns.

**Approaches: Linear Regression**:
In the realm of stock price prediction, two commonly employed approaches are Linear
Regression and Polynomial Regression. These regression techniques aim to establish a
mathematical relationship between input variables, such as historical stock prices and trading
volume, and the target variable, which is typically the future stock price. By fitting a regression
model to historical data, analysts can extrapolate this relationship to predict future price
movements. I will be using Linear Regression on this analysis.
**Target Variable and Inout Features**:
In the context of stock price prediction, the target variable is typically the future stock price that
analysts seek to predict. This could be the closing price of the stock on a future trading day. The
input variables, also known as features, are historical data points that serve as predictors for the
target variable. These can include past stock prices (e.g., open, high, low), trading volume, and
any other relevant financial indicators that may influence the future price movements of the
stock. By analyzing the historical relationship between these input variables and the target
variable, analysts can develop predictive models to forecast future stock prices.
Conclusion

### Linear Regression

So, I will be using Linear Regression and since we have multiple input featurs the formula will be:
- f(w , b) ( x)=w⋅ x+b=w1x1+w2x2+…+wnxn+b
- Here:
- f(w, b) = Representation of prediction made by Linear Regression
- w = weights assigned to each coefficient
- b = Bias Term/Intercept term
- x = input features where x1, x2, . .. , xn denotes individual features
- w1, ,. . .,wn = weights assigned to each feature
