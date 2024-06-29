## **Introduction:**

Hello everyone! 🌟 My name is Aditya, and I'd like to share some interesting findings from my research on how exchange rates (the value of one currency compared to another) change over time. 📉📈 I used a special method called Instrumented Principal Component Analysis (IPCA) to make sense of a lot of complex data. My research has shown some cool results that can help us better predict currency prices. This research won 2nd prize at the Undergraduate Research and Innovation Competition (URC), a prestigious national-level competition. 🏅

**About URC:**
The URC is the largest undergraduate research event in the entire GCC and MENA region, targeting all major disciplines. Last year, over 3000 research papers were presented from 27 disciplines by teams representing universities from 17 participating countries from across the region. 

### **Abstract:**
Predicting currency prices is like trying to predict the weather 🌦️—it's really tough! One reason is that the usual way of predicting assumes some key numbers (called beta coefficients) don't change over time ⏰. But guess what? They do! We used a special math trick called Instrumented Principal Component Analysis (IPCA) 🧩 first drafted by (Hsuan Fu, Shu-Fu Lee, Jui-Chung Yang - October 2023) to make sense of lots of data from different countries. Our new method did a better job at predicting than the old methods 🚀. We found out that things like medium-term interest rates, stock market trends 📊, and unique market movements 🌀 are super important for making accurate predictions.

### **Key Terminologies:**

1. **Foreign Exchange Market (FX):** This is where currencies are bought and sold. Think of it as a big marketplace where people trade money from different countries 💱.

2. **Beta Coefficients:** These are numbers that tell us how much a currency's price might change in response to changes in other factors 📈. Traditionally, they were assumed to stay the same over time, but we found out they actually change.

3. **Instrumented Principal Component Analysis (IPCA):** A fancy math method that helps us look at lots of data at once and find patterns 🧩. It's like having a super-smart assistant who can quickly spot important trends.

4. **Medium-term Interest Rate Differential:** The difference in interest rates between two countries over a medium period, like a few months or years. This can influence currency prices 📊.

5. **Stock Market Momentum:** This refers to the trend or direction in which the stock market is moving. If stocks are generally going up or down, it can affect currency prices 📉📈.

6. **Idiosyncratic Volatility:** Unique, unpredictable changes in the market that can affect currency prices 🌀.

---

## **Table of Contents:**

1. Introduction
   - Overview of the research
   - Purpose and significance

2. Abstract
   - Summary of findings

3. Key Terminologies
   - Explanation of important concepts

4. Section 1: Introduction to Foreign Exchange Markets
   - What is the foreign exchange market?
   - Importance of predicting exchange rates

5. Section 2: Traditional Prediction Methods
   - How beta coefficients were traditionally used
   - Limitations of old methods

6. Section 3: Introducing IPCA
   - What is IPCA?
   - How IPCA works

7. Section 4: Data Collection
   - Sources of data
   - Types of data used

8. Section 5: Empirical Findings
   - How IPCA performed compared to traditional methods
   - Key results and their significance

9. Section 6: Understanding the Results
   - Importance of medium-term interest rates
   - Role of stock market momentum
   - Impact of idiosyncratic volatility

10. Section 7: Practical Implications
    - How these findings can be used in real-world trading
    - Benefits for investors and financial analysts

11. Conclusion
    - Summary of key points
    - Future directions for research

12. References
    - Sources and further reading

---

| **Feature**                          | **PCA (Principal Component Analysis)**                                                                                      | **IPCA (Instrumented Principal Component Analysis)**                                                                     |
|--------------------------------------|----------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------|
| **Purpose**                          | Reduce the dimensionality of data by transforming it into a set of uncorrelated variables called principal components.       | Reduce dimensionality while also accounting for the changing relationships between variables over time.                   |
| **Method**                           | Identifies principal components based on the variance in the data without considering external instruments.                  | Identifies principal components by using instruments (additional variables) that help explain changes in the primary data. |
| **Beta Coefficients (Sensitivity)**  | Assumes beta coefficients (sensitivities) are constant over time.                                                           | Allows beta coefficients to change over time based on the instruments.                                                    |
| **Dynamic Capability**               | Static; does not adapt to changes in data relationships over time.                                                          | Dynamic; adapts to changes in data relationships over time, making it more flexible.                                      |
| **Data Usage**                       | Uses only the primary data set to identify principal components.                                                            | Uses both the primary data set and additional instruments to identify principal components.                               |
| **Example**                          | **PCA**: If we analyze a dataset of various fruit weights (apples, oranges, bananas), PCA would identify the main patterns in weight variance without considering seasonal changes or external factors. | **IPCA**: If we analyze the same fruit dataset, IPCA would consider external factors like seasonal weather conditions (instruments) that affect fruit weight, allowing for better understanding of how weights change over time. |
| **Application in Finance**           | **PCA**: Used to identify key factors driving market returns but assumes these factors remain constant.                     | **IPCA**: Used to identify key factors driving market returns while allowing these factors to change over time based on economic indicators (instruments). |
| **Predictive Power**                 | Good at explaining historical data but may not perform well in predicting future changes if relationships between variables change. | Better at predicting future changes due to its ability to adapt to evolving relationships between variables.             |
| **Example in Finance**               | **PCA**: Analyzing stock returns without considering time-varying factors like changing interest rates or economic policies. | **IPCA**: Analyzing stock returns while considering time-varying factors such as changes in interest rates or economic policies, providing a more accurate prediction of future returns. |

### Key Differences Explained with Examples

**PCA Example (Static Analysis)**:
- **Scenario**: You have data on fruit weights (apples, oranges, bananas) and want to identify the main patterns in their weights.
- **PCA Approach**: PCA will identify the main components that explain the most variance in fruit weights, but it won't account for external factors like seasonality. So, if apples are heavier in autumn, PCA won't adjust for this seasonal effect; it only focuses on the weight data as it is.

**IPCA Example (Dynamic Analysis with Instruments)**:
- **Scenario**: You have the same data on fruit weights, but you also have information on seasonal weather conditions that affect fruit growth.
- **IPCA Approach**: IPCA will use both the fruit weight data and the seasonal weather data as instruments to understand and predict changes in fruit weights over time. So, if apples are heavier in autumn due to favorable weather, IPCA will capture this relationship, providing a more nuanced understanding of weight changes.

In finance, this means IPCA can better account for how economic indicators (like interest rates) affect market returns over time, making it a more robust tool for predicting future changes compared to PCA, which assumes static relationships.
