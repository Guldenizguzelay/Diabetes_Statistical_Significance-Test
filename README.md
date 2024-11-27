# Diabetes Age Analysis: Statistical Significance Test
This project examines whether there is a statistically significant difference between the mean ages of individuals with diabetes and those without diabetes. The analysis includes hypothesis testing and assumption checks.

![image](https://github.com/user-attachments/assets/a012e8c1-5f5c-42ef-bd40-94ac1036ad02)

---

## Objective
The primary goal of this analysis is to test the following hypothesis:

* Null Hypothesis (H₀): There is no statistically significant difference in the mean ages between individuals with and without diabetes. (M₁ = M₂)
Alternative Hypothesis (H₁): There is a statistically significant difference in the mean ages between individuals with and without diabetes. (M₁ ≠ M₂)

## Dataset
The dataset used for this analysis is the Diabetes Dataset, which includes the following features:

* Outcome: Indicates whether an individual has diabetes (1 for diabetic, 0 for non-diabetic).
* Age: The age of the individual.
  
Sample Data:

![image](https://github.com/user-attachments/assets/4cbb7703-d730-4d5e-9381-8aa64516350c)

---

## Methodology
The analysis is performed in the following steps:

1. Data Loading and Exploration
   
The data is loaded using pandas and inspected for key insights such as the mean ages grouped by diabetes outcome.

3. Hypothesis Testing
   
Hypotheses:
*H₀: The mean ages of diabetic and non-diabetic individuals are equal.
*H₁: The mean ages of diabetic and non-diabetic individuals are not equal.

4. Assumption Checks
   
Normality Assumption:
The Shapiro-Wilk test is used to check if the data follows a normal distribution for each group (diabetic and non-diabetic).
If p-value > 0.05, the data follows a normal distribution.
If p-value ≤ 0.05, the data does not follow a normal distribution.

6. Non-Parametric Test
   
Since the normality assumption is violated, the Mann-Whitney U test is used as a non-parametric alternative to compare the two groups.

---

## Results

Normality Test (Shapiro-Wilk)

![image](https://github.com/user-attachments/assets/b32b7d73-b285-412c-b3e8-ca15541010f5)


Mann-Whitney U Test

![image](https://github.com/user-attachments/assets/0b738c37-1c05-443f-af67-9fa1a1e8a58f)

## Conclusion
Based on the Mann-Whitney U test results:

* If p-value ≤ 0.05: Reject H₀, indicating a statistically significant difference in the mean ages of diabetic and non-diabetic individuals.

* If p-value > 0.05: Fail to reject H₀, indicating no statistically significant difference.
