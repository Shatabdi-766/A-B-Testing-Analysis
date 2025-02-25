# 🎯 A/B Testing Analysis  
This project focuses on conducting A/B testing analysis using Python to evaluate and compare the performance of two distinct groups: the Control Group (Group A) and the Test Group (Group B). The analysis pipeline processes and examines the dataset to uncover meaningful insights into user behavior and identify statistically significant differences in performance metrics between the two groups.

## 📌 Project Overview :
A/B testing is a powerful statistical method used to compare two variations of a single variable to determine which performs better. This project implements a comprehensive A/B testing analysis pipeline, combining statistical methods and machine learning to evaluate the performance of Control (Group A) and Treatment (Group B) groups. The analysis focuses on key metrics such as impressions, clicks, purchases, and earnings, while leveraging advanced techniques to derive actionable insights and optimize outcomes.

**Designing A/B Tests** : 
- Setting up **control** and **treatment** groups effectively.  
- Ensuring **proper randomization** and **sample size determination**.  

**Data Analysis**  :
- Cleaning and preprocessing **experiment data**.  
- Visualizing trends and patterns for better insights.  

**Feature Engineering** : 
- Computing **derived metrics** such as:  
  - Conversion rate  
  - Earnings per purchase  
  - Other performance indicators  

**Statistical Testing** :  
- Conducting **hypothesis testing**, including:  
  - Normality tests  
  - Homogeneity tests  
  - Significance tests  
- Comparing groups to identify **statistically significant** differences.  

**Machine Learning Models** :  
- Predicting **user behavior**.  
- Identifying **key drivers** of performance.  
- Optimizing experiments using **predictive analytics**.  

**Visualization** :  
- Creating **intuitive plots and dashboards**.  
- Illustrating **data distributions**, test results, and insights.  

## Key Features :

1. **Data Loading and Inspection** :
  
   - Reads datasets for Group A and Group B from separate Excel sheets.

   - Explores data structure, types, and summary statistics to understand the dataset.

2. **Feature Engineering** :

    - Conversion Rate: Calculated as **(Purchases / Clicks) * 100**.

    - Earnings Per Purchase: Calculated as **Earnings / Purchases**.

3. **Data Visualization** :

    - Histograms and density plots to visualize metric distributions.

    - Box plots to compare group distributions.

4. **Statistical Analysis** :

    - **Shapiro-Wilk Test :** Checks for normality in the data.

    - **Levene’s Test :** Assesses homogeneity of variances.

    - **Independent t-tests :** For normally distributed data with equal variances.

     - **Mann-Whitney U Test :** For non-parametric data.

5. **Graphical Insights** : Generates graphs to compare impressions, clicks, purchases, earnings, conversion rates, and earnings per 
     purchase across groups.

6. **Performance Comparison** : Evaluates key metrics such as conversion rates, engagement levels, and user retention to compare the 
     effectiveness of Group A and Group B.

7. **Actionable Insights** : Provides data-driven recommendations to optimize strategies and improve outcomes based on the test results.

## 🛠 Tech Stack :
-  **Python-3.11** – Core language for analysis  
-  **Machine Learning** – Enhancing test results with predictive models  
-  **Pandas, NumPy, scipy** – Data manipulation & preprocessing  
-  **Matplotlib, Seaborn, termcolor** – Interactive visualizations
-  Google Colab

## Dataset :
The dataset used in this project is available in Excel(xlsx) format. You can download it [here](./ab_testing_data.xlsx). 

**The dataset consists of two groups** :

- **Control Group (Group A)**
- **Test Group (Group B)**

1. **Data Columns** :
  - Impression
  - Click
  - Purchase
  - Earning

2. **Calculated Metrics** :
  - Conversion Rate
  - Earnings per Purchase

## 🚀 Workflow :

## **Statistical Tests** :

- This project applies multiple statistical tests to validate hypotheses:

1. **Normality Test :**
    - **Shapiro-Wilk test :** Determines whether the data follows a normal distribution.
2. **Homogeneity of Variance Test :**
    - **Levene’s test :** Checks if the variances of the groups are equal.
3. **Parametric Tests (for normally distributed data with equal variances) :**
    - **Independent t-test :** Compares the means of two independent groups.
4. **Non-Parametric Tests (for non-normal data or unequal variances):**
   - **Mann-Whitney U test :** Compares the distributions of two independent groups when normality assumptions are not met.
  
## 📌 Key Findings and Insights : 

### 📊 Conversion Rate Analysis : 
- **Mann-Whitney U test** reveals a significant difference between **Group A** and **Group B**.  
- The **median conversion rate** of **Group B** is notably higher than that of **Group A**.  

### 📈 Other Metrics : 
- Detailed insights on:  
  - **Impressions**  
  - **Clicks**  
  - **Purchases**  
  - **Earnings**  
- Derived using suitable **statistical methods** for accurate analysis. 

## Output Samples :

### Controlled Group (Group A) :
| Impression      | Click         | Purchase      | Earning       |
|-----------------|---------------|---------------|---------------|
| 82529.459271    | 6090.077317   | 665.211255    | 2311.277143   |
| 98050.451926    | 3382.861786   | 315.084895    | 1742.806855   |
| 82696.023549    | 4167.965750   | 458.083738    | 1797.827447   |
| 109914.400398   | 4910.882240   | 487.090773    | 1696.229178   |
| 108457.762630   | 5987.655811   | 441.034050    | 1543.720179   |

### 📊 Dataset Overview: 
  - Controlled Group (Group A) Performance Metrics : The dataset provides performance metrics for **Group A** across four key areas: 
    **Impressions**, **Clicks**, **Purchases**, and **Earnings**.

### Test Group (Group B) :
| Impression | Click  | Purchase | Earning |
|------------|--------|----------|---------|
| 120104.0   | 3217.0 | 702.0    | 1940.0  |
| 134776.0   | 3635.0 | 834.0    | 2929.0  |
| 107807.0   | 3057.0 | 423.0    | 2526.0  |
| 116445.0   | 4650.0 | 429.0    | 2281.0  |
| 145083.0   | 5201.0 | 750.0    | 2782.0  |

## 📊 Dataset Overview: 
   - Test Group (Group B) Performance Metrics : The dataset provides performance metrics for **Group B** across four key areas: 
    **Impressions**, **Clicks**, **Purchases**, and **Earnings**.  

## Combined Dataset :
### Group A

| Impression      | Click         | Purchase      | Earning       | Conversion Rate | Earning Per Purchase | Group   |
|-----------------|---------------|---------------|---------------|-----------------|-----------------------|---------|
| 82529.459271    | 6090.077317   | 665.211255    | 2311.277143   | 10.922870       | 3.474501              | GroupA  |
| 98050.451926    | 3382.861786   | 315.084895    | 1742.806855   | 9.314152        | 5.531229              | GroupA  |
| 82696.023549    | 4167.965750   | 458.083738    | 1797.827447   | 10.990583       | 3.924670              | GroupA  |
| 109914.400398   | 4910.882240   | 487.090773    | 1696.229178   | 9.918600        | 3.482368              | GroupA  |
| 108457.762630   | 5987.655811   | 441.034050    | 1543.720179   | 7.365721        | 3.500229              | GroupA  |

### Group B

| Impression      | Click         | Purchase      | Earning       | Conversion Rate | Earning Per Purchase | Group   |
|-----------------|---------------|---------------|---------------|-----------------|-----------------------|---------|
| 79234.911929    | 6002.213585   | 382.047116    | 2277.863984   | 6.365104        | 5.962259              | GroupB  |
| 130702.239410   | 3626.320072   | 449.824592    | 2530.841327   | 12.404437       | 5.626285              | GroupB  |
| 116481.873365   | 4702.782468   | 472.453725    | 2597.917632   | 10.046259       | 5.498777              | GroupB  |
| 79033.834921    | 4495.428177   | 425.359102    | 2595.857880   | 9.462038        | 6.102744              | GroupB  |
| 102257.454089   | 4800.068321   | 521.310729    | 2967.518390   | 10.860486       | 5.692418              | GroupB  |

## 📊 Detailed Comparison: Group A vs Group B

The dataset provides a detailed comparison of **Group A** and **Group B** across key performance metrics, including **Impressions**, **Clicks**, **Purchases**, **Earnings**, **Conversion Rate**, and **Earning Per Purchase**. Here's a breakdown:

### 📌 Key Observations

#### **Group A**:
- **Impressions**: Ranges from 82,529 to 109,914  
- **Clicks**: Ranges from 3,383 to 6,091  
- **Purchases**: Ranges from 315 to 665  
- **Earnings**: Ranges from 1,543 to 2,311  
- **Conversion Rate**: Ranges from 7.37% to 10.99%  
- **Earning Per Purchase**: Ranges from 3.48 to 5.53  

#### **Group B**:
- **Impressions**: Ranges from 79,033 to 130,702  
- **Clicks**: Ranges from 3,626 to 6,002  
- **Purchases**: Ranges from 382 to 521  
- **Earnings**: Ranges from 2,277 to 2,967  
- **Conversion Rate**: Ranges from 6.37% to 12.40%  
- **Earning Per Purchase**: Ranges from 5.50 to 6.10  

### 📊 Comparison Between Groups :

#### **Impressions and Clicks**:
- Both groups have **similar ranges** for impressions and clicks.
- **Group A** has a **slightly higher Click-Through Rate (CTR)** on average.

#### **Purchases and Earnings**:
- **Group A** has **higher purchase numbers** in some cases (e.g., 665 vs. 521).
- **Group B** consistently generates **higher Earnings Per Purchase** (5.50–6.10 vs. 3.48–5.53).

#### **Conversion Rate**:
- **Group B** has a **higher maximum conversion rate** (12.40%) compared to **Group A** (10.99%).
- **Group A** has a **more consistent conversion rate** overall.

#### **Earning Per Purchase**:
- **Group B** outperforms **Group A** in **earnings per purchase**, indicating that **Group B customers** spend more per transaction.

### 🚀 Actionable Insights :

#### **For Group A**:
- Focus on **increasing Earnings Per Purchase** by **upselling** or **cross-selling** higher-value products.
- Maintain the strong **CTR** and **Conversion Rate**, but continue optimizing **ad creatives** and **targeting**.

#### **For Group B**:
- Leverage the higher **Earnings Per Purchase** to **maximize revenue**.
- Improve **CTR** to drive more clicks and purchases, as **Group B** lags slightly behind **Group A** in this area.

#### **Cross-Group Strategies**:
- **Combine the strengths of both groups**:  
  - Adopt **Group A's** higher **CTR** and more consistent **conversion rate**.  
  - Implement **Group B's** strategies for **higher earnings per purchase**.  

## 📊 Visualization Samples

### Example Graphs

#### **Histograms**:
- Compare the **distributions** of key metrics (e.g., **clicks**, **purchases**, **earnings**) for **Group A** and **Group B**.  
- These histograms provide insights into the **spread**, **skewness**, and **central tendencies** of the data, helping to identify patterns and anomalies.  
- Example:  
  - **Group A** may show a wider spread in earnings, while **Group B** could have a more concentrated distribution.

#### **Box Plots**:
- Visualize the **variance** and **central tendency** of metrics across both groups.  
- **Box plots** highlight **outliers**, **quartiles**, and **median values**, making it easier to compare the performance and **variability** between **Group A** and **Group B**.  
- Example:  
  - The **box plot** for **Group A** may show more variability in clicks, while **Group B** may have a higher median for earnings per purchase.

### **Impression**

![image](https://github.com/user-attachments/assets/daf908d4-46ff-4065-9492-f10623a7cce2)
![image](https://github.com/user-attachments/assets/974a3cae-b410-4cf5-9bec-c7c480fdf7f3)

### **Click**

![image](https://github.com/user-attachments/assets/ab433982-09b6-4b56-bcbb-9932d53ea5b1)
![image](https://github.com/user-attachments/assets/57a94842-c92d-47b0-9624-9887e1fa91b6)

### **Purchase**

![image](https://github.com/user-attachments/assets/abbf54de-fd58-4f94-be58-2519f1ab9ce9)
![image](https://github.com/user-attachments/assets/7821ae92-239b-4b9e-adcc-89c678bc0a5f)

### **Earning**

![image](https://github.com/user-attachments/assets/817e9a65-2e8f-44da-8c9a-d96a893845fc)
![image](https://github.com/user-attachments/assets/5f02dd3b-8a87-41d0-ba1f-3f6b63fae968)

### **Convertion Rate**

![image](https://github.com/user-attachments/assets/e461888b-be0e-48e3-b902-170e25d0dd37)
![image](https://github.com/user-attachments/assets/0f25b3fd-a009-4ec5-890b-ec133c8d6998)


### **Earning Per Purchase**
![image](https://github.com/user-attachments/assets/2f89d584-81f1-4cc2-b409-531b032e44c2)
![image](https://github.com/user-attachments/assets/abf223c6-2c10-4e32-9a23-ebb4c890e0d4)

## A/B Testing Summary Statistics

| Metric                   | Group   | count  | mean         | std           | median       | min            | max            |
|--------------------------|---------|--------|--------------|---------------|--------------|----------------|----------------|
| **Impression**            | GroupA  | 40     | 101711.45    | 20302.16      | 99790.70     | 45475.94       | 147539.34      |
|                          | GroupB  | 40     | 120512.41    | 18807.45      | 119291.30    | 79033.83       | 158605.92      |
| **Click**                 | GroupA  | 40     | 5100.66      | 1329.99       | 5001.22      | 2189.75        | 7959.13        |
|                          | GroupB  | 40     | 3967.55      | 923.10        | 3931.36      | 1836.63        | 6019.70        |
| **Purchase**              | GroupA  | 40     | 550.89       | 134.11        | 531.21       | 267.03         | 801.80         |
|                          | GroupB  | 40     | 582.11       | 161.15        | 551.36       | 311.63         | 889.91         |
| **Earning**               | GroupA  | 40     | 1908.57      | 302.92        | 1975.16      | 1253.99        | 2497.30        |
|                          | GroupB  | 40     | 2514.89      | 282.73        | 2544.67      | 1939.61        | 3171.49        |
| **Conversion Rate**       | GroupA  | 40     | 11.59        | 4.54          | 10.96        | 4.04           | 30.44          |
|                          | GroupB  | 40     | 15.66        | 6.82          | 14.62        | 6.37           | 44.79          |
| **Earning Per Purchase** | GroupA  | 40     | 3.69         | 1.14          | 3.49         | 1.83           | 6.71           |
|                          | GroupB  | 40     | 4.65         | 1.36          | 4.45         | 2.65           | 8.19           |

## 📊 Group A vs Group B: Performance Metrics Breakdown

### **Impression Insights**:
- **Group A** shows a **mean** of 101,711 impressions with a **range** of 45,475–147,539.
- **Group B** has a **higher mean** of 120,512, with impressions ranging from 79,033 to 158,606.  
- **Key Takeaway**: **Group B** consistently reaches a **larger audience**, evidenced by both a higher **mean** and **more consistent range**.

### **Click Performance**:
- **Group A** leads in **click volume** with an average of 5,101 clicks and a **range** of 2,190–7,959.
- **Group B**, however, shows a **mean** of 3,968 clicks, with a more **consistent** spread of 1,837–6,020.  
- **Key Takeaway**: While **Group A** has higher **clicks**, **Group B** has **stable** engagement, with fewer extreme variations.

### **Purchasing Behavior**:
- **Group A** achieves an average of 551 purchases, ranging from 267 to 802.
- **Group B** averages 582 purchases, spanning a range of 312–890.  
- **Key Takeaway**: **Group B** sees **slightly higher purchases**, but the **variability** in purchases is also more pronounced.

### **Revenue Generation**:
- **Group A** generates a **mean** of 1,909 in earnings, with a range between 1,254 and 2,497.
- **Group B** significantly outperforms, with a **mean** of 2,515 in earnings and a **range** of 1,940–3,171.  
- **Key Takeaway**: **Group B** not only earns **more**, but does so with **less variability**, showcasing a more **stable revenue generation** model.

### **Conversion Rate Comparison**:
- **Group A** has a **mean** conversion rate of 11.59%, with a range from 4.04% to 30.44%.
- **Group B** surpasses with a **mean** of 15.66%, fluctuating between 6.37% and 44.79%.  
- **Key Takeaway**: **Group B** excels with a **higher conversion rate**, although it experiences **greater variability**.

### **Earnings per Purchase**:
- **Group A** sees an average earning of 3.69 per purchase, ranging from 1.83 to 6.71.
- **Group B** generates **higher earnings per purchase**, averaging 4.65, with a range of 2.65–8.19.  
- **Key Takeaway**: **Group B** performs better in terms of **earnings per transaction**, but with **higher variability**.

---

## 🚀 Strategic Insights

### **For Group A**:
- Focus on improving **Earnings Per Purchase** and **Conversion Rate** to align more closely with **Group B**’s superior performance in these areas.

### **For Group B**:
- Leverage the **higher earnings per purchase** and **conversion rates**, while focusing on maintaining consistency in **click performance**.

### **Actionable Cross-Group Strategy**:
- **Combine the best of both groups** by utilizing **Group A's higher click volume** alongside **Group B's superior revenue and conversion rates** for optimal performance.






