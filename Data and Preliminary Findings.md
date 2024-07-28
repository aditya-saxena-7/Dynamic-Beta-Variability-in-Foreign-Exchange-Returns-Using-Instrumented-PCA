### 3. Data and Preliminary Findings 📊🔍

#### 3.1 Sources and Variable Definition 🌍📈

To understand how currency values change over time, we need a lot of data. Here's where we got our data and what each variable means:

**Data Sources 📅:**
We collected data from January 2008 to December 2020 from various sources. The data includes:
- **Foreign Exchange Rates 💱**: These are the values of different currencies relative to the US dollar.
- **Macroeconomic Data 📊**: Data on things like interest rates, inflation, and unemployment from different countries.

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

#### 3.2 Summary Statistics 📊📈

**Equally-Weighted Average Returns 📈**:
- **Definition**: The average return across all currencies in the G10 countries.
- **Example**: If the average return across these currencies is 1.2% per year, it means, on average, the value of these currencies increased by 1.2% annually.

**Standard Deviation 📉**:
- **Definition**: A measure of how much the currency returns vary from the average return.
- **Example**: A standard deviation of 10.9% means that the returns typically vary by 10.9% from the average, indicating volatility.

**Skewness 📉**:
- **Definition**: A measure of the asymmetry in the distribution of returns.
- **Example**: Positive skewness indicates more frequent small losses and a few large gains, while negative skewness indicates more frequent small gains and a few large losses.

**Kurtosis 📈**:
- **Definition**: A measure of the "tailedness" of the distribution of returns.
- **Example**: Positive kurtosis indicates a distribution with fat tails, meaning more extreme values (either gains or losses) than a normal distribution.

**Correlation Structures 📊**:
- **Definition**: How different variables move in relation to each other.
- **Example**: If the bill yield and bond yield have a high correlation (e.g., 80.5%), it means they tend to move together.

#### 3.3 Beta-Sorting Portfolios 📈📉

**Time-Varying Risk Premium 🌐🔄**:
- **Definition**: The additional return expected from holding a currency due to its risk, which changes over time.
- **Example**: If during one period, investing in the euro is considered riskier, the return expected from it might be higher to compensate for that risk.

**Sorting Currencies into Portfolios 📋**:
- **Process**: We divide the currencies into groups based on their beta coefficients. Currencies with similar betas are grouped together.
- **Example**: If we have 10 currencies, we might sort them into three portfolios: high-beta, medium-beta, and low-beta portfolios.

**Portfolio Characteristics 📈**:
- **Observation**: Betas in the high group decrease and those in the low group increase over time.
- **Example**: If the average beta for a high-beta portfolio decreases from 1.5 to 1.2, and for a low-beta portfolio, it increases from 0.5 to 0.8, it indicates that the sensitivity to underlying factors changes over time.

**IPCA Model Advantages 🧩**:
- **Definition**: The IPCA model allows beta coefficients to change over time based on economic conditions, improving prediction accuracy.
- **Example**: During a financial crisis, the sensitivity of currencies to interest rates might increase, and the IPCA model can capture this change.

## **Table of Contents:**

1. [Introduction](https://github.com/aditya-saxena-7/Dynamic-Beta-Variability-in-Foreign-Exchange-Returns-Using-Instrumented-PCA/blob/main/Introduction.md)

2. [Methodology](https://github.com/aditya-saxena-7/Dynamic-Beta-Variability-in-Foreign-Exchange-Returns-Using-Instrumented-PCA/blob/main/Methodology.md)

3. [Data and Preliminary Findings](https://github.com/aditya-saxena-7/Dynamic-Beta-Variability-in-Foreign-Exchange-Returns-Using-Instrumented-PCA/blob/main/Data%20and%20Preliminary%20Findings.md)

4. [Empirical Findings](https://github.com/aditya-saxena-7/Dynamic-Beta-Variability-in-Foreign-Exchange-Returns-Using-Instrumented-PCA/blob/main/Empirical%20Findings.md)

5. [Interpreting IPCA Factors](https://github.com/aditya-saxena-7/Dynamic-Beta-Variability-in-Foreign-Exchange-Returns-Using-Instrumented-PCA/blob/main/Interpreting%20IPCA%20Factors.md)

6. [Robustness and discussions](https://github.com/aditya-saxena-7/Dynamic-Beta-Variability-in-Foreign-Exchange-Returns-Using-Instrumented-PCA/blob/main/Robustness%20and%20discussions.md)

7. [Conclusion](https://github.com/aditya-saxena-7/Dynamic-Beta-Variability-in-Foreign-Exchange-Returns-Using-Instrumented-PCA/blob/main/Conclusion.md)
