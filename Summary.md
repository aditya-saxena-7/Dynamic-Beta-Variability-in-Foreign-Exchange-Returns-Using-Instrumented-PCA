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
