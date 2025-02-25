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

5. **Graphical Insights** : Generates graphs to compare impressions, clicks, purchases, earnings, conversion rates, and earnings per purchase across groups.

6. **Performance Comparison** : Evaluates key metrics such as conversion rates, engagement levels, and user retention to compare the effectiveness of Group A and Group B.

7. **Actionable Insights** : Provides data-driven recommendations to optimize strategies and improve outcomes based on the test results.

## 🛠 Tech Stack :
-  **Python-3.11** – Core language for analysis  
-  **Machine Learning** – Enhancing test results with predictive models  
-  **Pandas, NumPy, scipy** – Data manipulation & preprocessing  
-  **Matplotlib, Seaborn, termcolor** – Interactive visualizations
-  Google Colab

## Dataset :
The dataset used in this project is available in CSV format. You can download it [here](./sales_retail_II_cleaned.zip).

## 🚀 Workflow :

