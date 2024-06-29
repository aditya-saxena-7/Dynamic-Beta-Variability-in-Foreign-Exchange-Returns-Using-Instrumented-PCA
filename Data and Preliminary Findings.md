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

---

### Summary Statistics 📊📈

**1. Average Returns Across Currencies 🌍💵:**
- **Finding**: The equally-weighted average return across the G10 currencies is 1.2% per year.
- **Layman Explanation**: If you invested in a mix of these 10 different currencies, on average, you would earn a 1.2% return each year. This means the overall value of these currencies increased by 1.2% annually.
- **Example**: Imagine you have a basket of different fruits. If the average weight of the fruits increases by 1.2% each year, it means, on average, each fruit is getting slightly heavier each year.

**2. Standard Deviation 📉:**
- **Finding**: The standard deviation of returns is 10.9% per year.
- **Layman Explanation**: This number tells us how much the currency returns typically vary from the average return. A higher standard deviation means more volatility, or bigger ups and downs in the returns.
- **Example**: If the weight of your basket of fruits fluctuates by 10.9% from the average each year, it means some years the fruits might be much heavier or lighter than the average weight.

**3. Skewness 📉:**
- **Finding**: The skewness of the returns is mostly positive.
- **Layman Explanation**: Positive skewness indicates that there are more frequent small losses and a few large gains in currency returns. This means that while most of the time the returns might be small, occasionally, there can be significant gains.
- **Example**: If your fruit basket usually gains a small amount of weight, but occasionally you get a really big, heavy fruit, that's positive skewness.

**4. Kurtosis 📈:**
- **Finding**: The kurtosis of the returns is positive.
- **Layman Explanation**: Positive kurtosis indicates that the distribution of returns has "fat tails," meaning there are more extreme values (big gains or losses) than in a normal distribution.
- **Example**: If most of your fruits are average-sized, but occasionally you get some really big or really small fruits, that's positive kurtosis.

**5. Correlation Structures 📊:**
- **Finding**: There are high correlations among bond-based variables, and moderate correlations between other variables like stock market momentum and dividend yield.
- **Layman Explanation**: High correlation means that certain variables tend to move together. For example, if short-term interest rates (bills) go up, medium-term (notes) and long-term (bonds) interest rates also go up. Moderate correlation means the relationship is less strong but still noticeable.
- **Example**: If the price of apples and oranges in your fruit basket tend to rise and fall together, that's high correlation. If apples and bananas have a weaker but still noticeable relationship, that's moderate correlation.

### Beta-Sorting Portfolios 📈📉

**1. Time-Varying Risk Premium 🌐🔄:**
- **Finding**: The risk premium (extra return for taking on risk) in the foreign exchange market changes over time.
- **Layman Explanation**: The amount of extra return you get for investing in riskier currencies isn't constant; it varies. Sometimes you get more extra return for the risk, sometimes less.
- **Example**: If you sometimes get a higher reward for eating a particularly spicy fruit, and other times the reward is less, the "spiciness" reward is changing over time.

**2. Sorting Currencies into Portfolios 📋:**
- **Finding**: Currencies are sorted into high-beta, medium-beta, and low-beta portfolios based on their sensitivity to underlying factors.
- **Layman Explanation**: Currencies are grouped based on how sensitive they are to different economic factors. High-beta currencies are more sensitive, while low-beta currencies are less sensitive.
- **Example**: If some fruits in your basket respond more to sunlight (high-beta) and others less (low-beta), you group them accordingly.

**3. Portfolio Characteristics 📈:**
- **Finding**: Betas in the high group tend to decrease over time, while betas in the low group tend to increase.
- **Layman Explanation**: Over time, the sensitivity of high-beta currencies to economic factors tends to go down, while the sensitivity of low-beta currencies goes up.
- **Example**: If your sun-sensitive fruits become less responsive to sunlight over time, and the less sun-sensitive fruits become more responsive, that's similar to how betas are changing.

**4. IPCA Model Advantages 🧩:**
- **Finding**: The IPCA model allows beta coefficients to change over time based on economic conditions, improving prediction accuracy.
- **Layman Explanation**: The IPCA model can adapt to changes in economic conditions by adjusting the sensitivity of currencies to various factors. This makes the model more accurate in predicting currency returns.
- **Example**: If your fruit basket can adjust how it reacts to sunlight based on the season, it will be better at predicting how the fruits will grow.
