## Dynamic Beta Variability in Foreign Exchange Returns Using Instrumented PCA
---

### Table of Contents:

1. [Introduction](https://github.com/aditya-saxena-7/Dynamic-Beta-Variability-in-Foreign-Exchange-Returns-Using-Instrumented-PCA/blob/main/Introduction.md)

2. [Methodology](https://github.com/aditya-saxena-7/Dynamic-Beta-Variability-in-Foreign-Exchange-Returns-Using-Instrumented-PCA/blob/main/Methodology.md)

3. [Data and Preliminary Findings](https://github.com/aditya-saxena-7/Dynamic-Beta-Variability-in-Foreign-Exchange-Returns-Using-Instrumented-PCA/blob/main/Data%20and%20Preliminary%20Findings.md)

4. [Empirical Findings](https://github.com/aditya-saxena-7/Dynamic-Beta-Variability-in-Foreign-Exchange-Returns-Using-Instrumented-PCA/blob/main/Empirical%20Findings.md)

5. [Interpreting IPCA Factors](https://github.com/aditya-saxena-7/Dynamic-Beta-Variability-in-Foreign-Exchange-Returns-Using-Instrumented-PCA/blob/main/Interpreting%20IPCA%20Factors.md)

6. [Robustness and discussions](https://github.com/aditya-saxena-7/Dynamic-Beta-Variability-in-Foreign-Exchange-Returns-Using-Instrumented-PCA/blob/main/Robustness%20and%20discussions.md)

7. [Conclusion](https://github.com/aditya-saxena-7/Dynamic-Beta-Variability-in-Foreign-Exchange-Returns-Using-Instrumented-PCA/blob/main/Conclusion.md)

### Abstract:
Predicting currency prices is like trying to predict the weather 🌦️—it's really tough! One reason is that the usual way of predicting assumes some key numbers (called beta coefficients) don't change over time ⏰. But guess what? They do! We used a special math trick called Instrumented Principal Component Analysis (IPCA) 🧩 first drafted by (Hsuan Fu, Shu-Fu Lee, Jui-Chung Yang - October 2023) to make sense of lots of data from different countries. Our new method did a better job at predicting than the old methods 🚀. We found out that things like medium-term interest rates, stock market trends 📊, and unique market movements 🌀 are super important for making accurate predictions.

In finance, this means IPCA can better account for how economic indicators (like interest rates) affect market returns over time, making it a more robust tool for predicting future changes compared to PCA, which assumes static relationships.

### Key Terminologies:

1. **Foreign Exchange Market (FX):** This is where currencies are bought and sold. Think of it as a big marketplace where people trade money from different countries 💱.

2. **Beta Coefficients:** These are numbers that tell us how much a currency's price might change in response to changes in other factors 📈. Traditionally, they were assumed to stay the same over time, but we found out they actually change.

3. **Medium-term Interest Rate Differential:** The difference in interest rates between two countries over a medium period, like a few months or years. This can influence currency prices 📊.

4. **Stock Market Momentum:** This refers to the trend or direction in which the stock market is moving. If stocks are generally going up or down, it can affect currency prices 📉📈.

5. **Idiosyncratic Volatility:** Unique, unpredictable changes in the market that can affect currency prices 🌀.

### Objective:

The foreign exchange (FX) market is where different currencies are traded. Imagine you're traveling from the USA to Europe and need to exchange your dollars for euros. The rate at which you exchange these currencies is determined in the FX market. 

**Why is it Challenging? 🤔**

1. **Random Walk Theory 🚶‍♂️**: One reason predicting FX rates is tough is because they often seem to follow a "random walk" pattern. This theory suggests that changes in exchange rates are random and unpredictable, much like how you might wander around aimlessly without a clear direction. 

2. **Changing Predictors 🔄**: Another reason is that the factors influencing FX rates can change over time. Factors like interest rates, economic growth, and political stability can all impact currency values, but their influence can vary. 

**Why Do We Care About Predicting FX Rates? 📊**

Despite the difficulties, predicting FX rates is crucial. The FX market is massive, with a trading volume of about $7.5 trillion per day as of 2022. Accurate predictions can help investors make better decisions, businesses plan for currency fluctuations, and governments manage their economies more effectively.

**Real-World Examples 🌐**

Imagine a company that imports goods from different countries. If the company can accurately predict future exchange rates, it can decide when to buy foreign currency and save money. For instance, if it knows that the euro will strengthen against the dollar, it can buy euros in advance. Similarly, an investor can use these predictions to choose the best times to trade currencies and maximize profits.

**Traditional Prediction Methods and Their Limitations 📉**

In the past, many models assumed that certain key numbers (beta coefficients) that describe how FX rates respond to different factors stayed constant over time. However, this assumption doesn't hold true in the real world, leading to inaccurate predictions.

**Our Approach: Instrumented Principal Component Analysis (IPCA) 🧩**

To tackle this problem, we used a method called Instrumented Principal Component Analysis (IPCA). This technique helps us look at lots of data and find important patterns, even when those patterns change over time. It's like having a super-smart assistant who can quickly spot trends in a sea of information.

**Advantages of IPCA 🚀**

- **Flexibility**: Unlike traditional models, IPCA allows the beta coefficients to change over time, making it more adaptable to real-world conditions.
- **Efficiency**: By using data from multiple countries and various economic factors, IPCA can make more accurate predictions.
- **Better Performance**: Our results showed that IPCA outperformed traditional models in predicting FX rates.

**Why Betas Matter in Our Model 📉➡️📈**

- **Beta Coefficients**: These numbers tell us how much an FX rate will change in response to changes in other factors (like interest rates or economic growth). In traditional models, these were assumed to be constant, but we found that they actually vary over time.
- **Time-Varying Betas**: By allowing betas to change, our model can adapt to different economic conditions, leading to more accurate predictions.

**Data Collection 📅📈**

We collected data on exchange rates and various economic factors from G10 countries (Australia, Canada, Switzerland, Denmark, Euro Area, UK, Japan, Norway, New Zealand, and Sweden) from January 2008 to December 2020. This gives us a broad and diverse dataset to work with.

**Currencies from G10 Countries 🌐:**
The G10 countries are:
- Australia 🇦🇺
- Canada 🇨🇦
- Switzerland 🇨🇭
- Denmark 🇩🇰
- Euro Area 🇪🇺
- United Kingdom 🇬🇧
- Japan 🇯🇵
- Norway 🇳🇴
- New Zealand 🇳🇿
- Sweden 🇸🇪

**Variables and Their Definitions 📋:**

1. **Inflation Differential (INFi,t) 📈🔄**: 
   - **Definition**: The difference in inflation rates between a country and the US.
   - **Example**: If the inflation rate in the US is 2% and in Canada it's 3%, the inflation differential is 1%. Higher inflation in a country typically weakens its currency.

2. **Unemployment Rate Gap Differential (UNi,t) 💼📉**:
   - **Definition**: The difference in the unemployment rate gap (cyclical component) between a country and the US.
   - **Example**: If the unemployment rate in the US is 5% and in Japan it's 4%, and considering economic cycles, the differential helps understand economic health.

3. **Bill Yield Differential (BILLi,t) 📈📊**:
   - **Definition**: The difference in short-term interest rates (three-month government bills) between a country and the US.
   - **Example**: If short-term interest rates are higher in the US than in Canada, it can make US investments more attractive, affecting currency values.

4. **Note Yield Differential (NOTEi,t) 📈📝**:
   - **Definition**: The difference in medium-term interest rates (five-year government debt) between a country and the US.
   - **Example**: If the five-year interest rate in the UK is higher than in the US, it might attract more investments to the UK, strengthening the pound.

5. **Bond Yield Differential (BONDi,t) 📈💵**:
   - **Definition**: The difference in long-term interest rates (ten-year government bonds) between a country and the US.
   - **Example**: Higher long-term interest rates in a country can attract long-term investments, affecting its currency value.

6. **Dividend Yield Differential (DPi,t) 💰📊**:
   - **Definition**: The difference in dividend yields (returns from stocks) between a country and the US.
   - **Example**: If stocks in Australia offer higher dividends than US stocks, investors might prefer Australian stocks, affecting the Australian dollar.

7. **Price-Earnings Differential (PEi,t) 📈💼**:
   - **Definition**: The difference in price-earnings ratios (valuation of stocks) between a country and the US.
   - **Example**: If stocks in Europe are cheaper relative to their earnings compared to US stocks, it might attract investments to Europe, influencing the euro.

8. **Stock Market Momentum Differential (SRET12i,t) 📈📉**:
   - **Definition**: The difference in the 12-month cumulative returns of stock indices between a country and the US.
   - **Example**: If Japanese stocks have been performing better than US stocks over the past year, it could strengthen the yen.

9. **Idiosyncratic Volatility (IVi,t) 📉🔄**:
   - **Definition**: The unique, unpredictable changes in the market that affect currency values.
   - **Example**: Unexpected political events in Canada can cause unpredictable changes in the Canadian dollar.

10. **Idiosyncratic Skewness (ISi,t) 📉🌀**:
    - **Definition**: The skewness (asymmetry) in the distribution of currency returns.
    - **Example**: If the returns on the Swiss franc tend to be more positive or negative in an unexpected way, it reflects in the skewness.

**Key Findings 🔍**

1. **Interest Rate Differential**: The difference in interest rates between two countries over a medium period is a crucial factor.
2. **Stock Market Momentum**: Trends in the stock market also play a significant role.
3. **Idiosyncratic Volatility**: Unique, unpredictable changes in the market impact FX rates.

**Overview of Instrumented Principal Component Analysis (IPCA) 🧩**

(Add link here about PCA vs IPCA)

**Factor Model for Currency Returns 💹**

In finance, a **factor model** is used to explain the returns (profits or losses) on investments based on various factors. For example, factors might include things like interest rates, inflation, or stock market performance. 

**Key Components of Our Model 🔑**

**1. Currency Return (ri,t+1) 💵➡️📈**
- **Definition**: Currency return refers to how much the value of a currency changes over a specific period.
- **Example**: Imagine you invest in euros (EUR) at the start of the month. By the end of the month, the value of the euros you hold has increased by 2%. This 2% change is the currency return.

**2. Beta Coefficients (βi,t) 📈➡️💵**
- **Definition**: Beta coefficients are numbers that measure the sensitivity of the currency return to changes in underlying factors. Think of them as "sensitivity dials" that adjust how strongly different factors affect the currency return.
- **Example**: If the beta coefficient for interest rates (one of the factors) is 0.5, it means that for every 1% change in interest rates, the currency return changes by 0.5%. If the interest rate increases by 2%, the currency return would increase by 1% (0.5 * 2%).

**3. Latent Factors (ft+1) 🔍**
- **Definition**: Latent factors are hidden or underlying variables that influence currency returns. These factors are not directly observed but can be inferred from the data.
- **Example**: Some latent factors might include economic growth, geopolitical events, or changes in investor sentiment. For instance, if there's a major geopolitical event, it might affect currency values, even though the exact impact (latent factor) isn't directly measured.

**4. Error Term (ϵi,t+1) ❌**
- **Definition**: The error term represents the part of the currency return that cannot be explained by the model. It's the "noise" or random fluctuations that are unpredictable.
- **Example**: If you predicted the currency return to be 2%, but it actually turns out to be 2.5%, the extra 0.5% is the error term. This could be due to random market movements or unexpected news.

**Dynamic Factor Loadings 🔄**

In traditional models, beta coefficients are assumed to be constant, like fixed dials on a machine. However, in reality, these coefficients can change over time based on economic conditions. Our model allows these "volume knobs" (beta coefficients) to move up and down as conditions change, making our predictions more accurate.

**Country Characteristics as Instruments 🌍📊**

We use specific characteristics of countries (like interest rates, inflation rates, etc.) as instruments to help our model. 

(Add Math IPCA)

## Module 3: Combining PCA with Instrumental Variables (IPCA)

### 2. The IPCA Algorithm
#### 4.1 Step-by-Step IPCA Algorithm
The IPCA algorithm involves the following steps:

#### 2.1 Data Preparation
- **Collect and Standardize Data**: The paper collects FX spot and forward rates from Datastream, covering the period from January 2008 to December 2020, for G10 countries. They standardize the data to ensure consistency.
- **Identify Instrumental Variables**: The study uses macroeconomic and financial variables such as interest rate differentials, stock market momentum, and idiosyncratic volatility as instrumental variables.

#### 2.2 Model Specification
- **Define the Model**: The IPCA model is specified to account for time-varying betas by incorporating country-specific characteristics into the factor model. The model equation is:
  \[
  r_{i,t+1} = \alpha_{i,t} + \beta_{i,t} f_{t+1} + \epsilon_{i,t+1}
  \]
  where \( r_{i,t+1} \) is the return of asset \( i \) at time \( t+1 \), \( \alpha_{i,t} \) is the intercept, \( \beta_{i,t} \) are the factor loadings, and \( f_{t+1} \) are the latent factors.
- **Select Instruments**: Instruments \( Z_{i,t} \) are selected to ensure they are correlated with the endogenous variables and uncorrelated with the error term. The characteristics \( z_{i,t} \) include macroeconomic conditions and financial indicators.

#### 2.3 First Stage Regression
- **Regress Endogenous Variables on Instruments**: Each endogenous variable is regressed on the instrumental variables to isolate the exogenous variation. The first stage regression is:
  \[
  X_i = \pi_0 + \pi_1 Z_1 + \pi_2 Z_2 + \cdots + \pi_k Z_k + u
  \]
- **Obtain Predicted Values**: The fitted values from the regression are used to create instrumented versions of the endogenous variables.

#### 2.4 Constructing the Instrumented Data
- **Create Instrumented Variables**: Use the fitted values \( \hat{X} \) from the first stage regression to construct the instrumented data \( \hat{X}_i \).

#### 2.5 Principal Component Analysis on Instrumented Data
- **Compute Covariance Matrix**: Calculate the covariance matrix of the instrumented data \( \hat{X}_i \).
- **Eigenvalue Decomposition**: Perform eigenvalue decomposition on the covariance matrix to obtain eigenvalues and eigenvectors.
- **Select Principal Components**: Choose the principal components with the largest eigenvalues, explaining the most variance in the data.
- **Project Data onto Principal Components**: Project the original data onto the selected principal components to reduce dimensionality.
  
### 3. Applying IPCA to FX Returns

#### 3.1 Empirical Implementation
- **Model Estimation**: The paper estimates the IPCA model by combining the instrumented variables and performing PCA. This allows for the extraction of latent factors that account for time-varying betas.
  
- **Validation and Testing**: The model's performance is validated using both in-sample and out-of-sample tests. The IPCA model demonstrates superior predictive power compared to traditional PCA and random walk models.

##### Step 6: Model Estimation and Validation
1. **Model Estimation**:
   - Estimate the IPCA model by combining the instrumented variables and performing PCA. This involves solving the optimization problem to minimize the sum of squared residuals subject to constraints on the factor loadings.
     \[
     \min_{\Gamma_{\beta}, \Gamma_{\alpha}, F} \sum_{t=1}^{T-1} (r_{t+1} - Z_t \Gamma_{\alpha} - Z_t \Gamma_{\beta} f_{t+1})^T (r_{t+1} - Z_t \Gamma_{\alpha} - Z_t \Gamma_{\beta} f_{t+1})
     \]
   - Where \( r_{t+1} \) is the return vector, \( Z_t \) is the matrix of country characteristics, \( \Gamma_{\alpha} \) and \( \Gamma_{\beta} \) are coefficient matrices, and \( f_{t+1} \) are the latent factors.

2. **Validation and Testing**:
   - Evaluate the model's performance using in-sample and out-of-sample tests.
   - Compare the predictive power of the IPCA model with benchmarks like the random walk model and traditional PCA.

#### 3.2 Key Findings

- **Out-of-Sample Predictability**: IPCA outperforms the random walk and PCA models in terms of out-of-sample predictability, indicating its robustness in capturing time-varying risk premiums.
- **Significance of Instrumental Variables**: The study finds that interest rate differentials, stock market momentum, and idiosyncratic volatility are significant predictors of FX returns, confirming the effectiveness of the chosen instruments.

### 4. Practical Implementation of IPCA in Python (Contextual Example)
Below is a practical example of implementing the IPCA algorithm in Python, contextualized for the research paper's FX returns analysis:

```python
import numpy as np
from sklearn.linear_model import LinearRegression
from sklearn.decomposition import PCA
from sklearn.preprocessing import StandardScaler

# Step 1: Data Preparation
# Example data (X: endogenous variables, Z: instrumental variables)
# Assume X and Z are pre-collected and standardized data arrays
X = np.random.rand(100, 2)  # Placeholder for actual FX returns data
Z = np.random.rand(100, 2)  # Placeholder for actual instrumental variables

# Standardize the data
scaler = StandardScaler()
X_scaled = scaler.fit_transform(X)
Z_scaled = scaler.fit_transform(Z)

# Step 2: First Stage Regression
# Regress each endogenous variable on the instruments
reg1 = LinearRegression().fit(Z_scaled, X_scaled[:, 0])
X1_hat = reg1.predict(Z_scaled)

reg2 = LinearRegression().fit(Z_scaled, X_scaled[:, 1])
X2_hat = reg2.predict(Z_scaled)

# Step 3: Constructing the Instrumented Data
X_hat = np.column_stack((X1_hat, X2_hat))

# Step 4: Principal Component Analysis on Instrumented Data
# Compute covariance matrix
cov_matrix = np.cov(X_hat, rowvar=False)

# Eigenvalue decomposition
eigenvalues, eigenvectors = np.linalg.eigh(cov_matrix)

# Select principal components (e.g., select top 2 components)
num_components = 2
principal_components = eigenvectors[:, -num_components:]

# Project data onto principal components
X_reduced = X_hat.dot(principal_components)

print("Reduced-dimensional representation:\n", X_reduced)
```

### Detailed Example

Let's walk through a simplified example using interest rate differentials:

1. **Data Collection**:
   - Collect monthly returns for the Euro (EUR/USD) from 2008 to 2020.
   - Gather economic indicators like the interest rate differential between the Eurozone and the US, stock market momentum, and idiosyncratic volatility.

2. **Define the Factor Model**:
   - Assume the Euro's return is influenced by a common factor (e.g., global economic condition) and a base return.
   - The factor model is:
     \[
     r_{\text{EUR},t+1} = \alpha_{\text{EUR},t} + \beta_{\text{EUR},t} f_{t+1} + \epsilon_{\text{EUR},t+1}
     \]

3. **Dynamic Factor Loadings**:
   - Allow the base return (\( \alpha_{\text{EUR},t} \)) and the sensitivity to the common factor (\( \beta_{\text{EUR},t} \)) to vary based on current economic indicators:
     \[
     \alpha_{\text{EUR},t} = z_{\text{EUR},t}^\top \Gamma_\alpha + \nu_{\alpha,\text{EUR},t}
     \]
     \[
     \beta_{\text{EUR},t} = z_{\text{EUR},t}^\top \Gamma_\beta + \nu_{\beta,\text{EUR},t}
     \]

4. **Observable Characteristics**:
   - Let \( z_{\text{EUR},t} \) include the medium-term interest rate differential, stock market momentum, and idiosyncratic volatility.
   - For instance, if the medium-term interest rate differential increases, the model will adjust the factor loading (\( \beta_{\text{EUR},t} \)) to reflect this new information.

5. **Combining the Model**:
   - Substitute the dynamic expressions into the factor model:
     \[
     r_{\text{EUR},t+1} = z_{\text{EUR},t}^\top \Gamma_\alpha + z_{\text{EUR},t}^\top \Gamma_\beta f_{t+1} + \epsilon^*_{\text{EUR},t+1}
     \]
   - This combined model now accounts for changing economic conditions and their impact on the Euro's returns.

**Comparing In-Sample and Out-of-Sample Performance 📊🔄**

- **PCA vs. IPCA**: PCA might look better during training (higher Total R²) but doesn’t predict future returns well (negative Predictive R²). IPCA, on the other hand, balances fitting historical data and predicting future returns better.
  
- **Example**: If you have two cookie recipes, PCA might be great for your initial batch (training), but when you try it on new ingredients (testing), it fails. IPCA, while not perfect in the initial batch, performs better with new ingredients.

#### 4.3 Economic Significance Based on the IPCA Predictions 💼📈

**Trading Strategies Based on Predictions 📊💹**

- **Definition**: We use the predicted returns from the IPCA model to create trading strategies. If the model predicts a currency will go up, we buy that currency (long position). If it predicts a drop, we sell that currency (short position).
- 
- **Example**: If the IPCA model predicts the euro will rise, we buy euros. If it predicts the yen will fall, we sell yen.
  
- **Findings**: The IPCA model generally outperforms PCA in both full-sample and out-of-sample periods, meaning it provides better trading signals.

**Portfolio Performance 📈📉**

- **Equally-Weighted Portfolio**: We create a portfolio by equally weighting the returns of all ten currencies.
  
- **Findings**: The IPCA model yields better returns than PCA. While PCA might show some good fits during training, it doesn't translate to actual economic gains when tested with new data.
