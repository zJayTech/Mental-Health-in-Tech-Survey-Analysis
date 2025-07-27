# Mental Health in Tech Survey Analysis

## Project Overview

This project analyzes a dataset on mental health in the tech industry, sourced from Kaggle. The objective is to explore various factors related to mental health attitudes, prevalence of mental health conditions, and support systems within tech companies. Through this analysis, we aim to uncover trends, correlations, and key insights that shed light on the state of mental health awareness and support in the tech sector.

## Dataset

The dataset used for this analysis is the [OSMI Mental Health in Tech Survey](https://www.kaggle.com/datasets/osmi/mental-health-in-tech-survey), originally from a Kaggle survey on Mental Health in Tech. It contains responses from individuals covering a range of topics including demographics, employment details, family history of mental illness, company benefits, attitudes towards mental health, and personal experiences.

## Tools and Technologies

* **RStudio:** Integrated Development Environment for R.
* **R:** Programming language for statistical computing and graphics.
* **`ggplot2`:** Powerful R package for creating elegant and informative data visualizations.
* **`dplyr`:** R package for data manipulation and transformation.
* **`forcats`:** R package for handling categorical variables (factors).

## Analysis and Visualizations

This section showcases the key visualizations generated during the analysis, along with explanations of the insights derived from each.

---

### 1. Gender Distribution

This bar chart illustrates the overall distribution of respondents by gender, providing a foundational understanding of the survey's demographic makeup.

![Gender Distribution](images/gender_distribution.png)
*(Please replace this placeholder with your actual plot image: `gender_distribution.png`)*

> **Insight:** The survey primarily reflects responses from male individuals, indicating a potential bias towards male perspectives in the tech industry data.

---

### 2. Mental Health Treatment by Gender

This visualization explores the proportion of individuals who sought mental health treatment, broken down by gender.

![Treatment by Gender](images/treatment_by_gender.png)
*(Please replace this placeholder with your actual plot image: `treatment_by_gender.png`)*

> **Insight:** While males constitute the majority of respondents, a higher proportion of female respondents reported seeking mental health treatment, suggesting potential differences in help-seeking behaviors.

---

### 3. Mental Health Treatment by Tech Company Affiliation

This chart investigates whether working for a tech company influences an individual's likelihood of seeking mental health treatment.

![Treatment by Tech Company](images/treatment_by_tech_company.png)
*(Please replace this placeholder with your actual plot image: `treatment_by_tech_company.png`)*

> **Insight:** Individuals working in tech companies appear to seek treatment more frequently, which might be attributed to greater awareness, resources, or perhaps higher stress levels within the industry.

---

### 4. Proportion of Treatment by Company Benefits

This stacked bar chart shows the proportion of respondents who sought treatment, categorized by the types of mental health benefits their company provides.

![Benefits vs. Treatment](images/benefits_vs_treatment.png)
*(Please replace this placeholder with your actual plot image: `benefits_vs_treatment.png`)*

> **Insight:** Companies offering comprehensive mental health benefits show a higher proportion of employees seeking treatment, indicating that accessible benefits play a crucial role in encouraging help-seeking behavior.

---

### 5. Age Distribution

A histogram showing the age distribution of the survey respondents. This helps in understanding the age groups most represented in the survey.

![Age Distribution](images/age_distribution.png)
*(Please replace this placeholder with your actual plot image: `age_distribution.png`)*

> **Insight:** The majority of respondents fall within the 25-40 age bracket, suggesting that mental health concerns in this survey are predominantly observed among younger to middle-aged professionals.

---

### 6. Self-Employed Distribution

This pie chart visualizes the proportion of self-employed individuals versus those employed by companies in the dataset.

![Self-Employed Distribution](images/self_employed_distribution.png)
*(Please replace this placeholder with your actual plot image: `self_employed_distribution.png`)*

> **Insight:** The vast majority of respondents are not self-employed, indicating that the survey primarily captures experiences from individuals working for established companies.

---

### 7. Family History of Mental Illness

This pie chart illustrates the proportion of respondents who have a family history of mental illness.

![Family History Distribution](images/family_history_distribution.png)
*(Please replace this placeholder with your actual plot image: `family_history_distribution.png`)*

> **Insight:** A significant portion of respondents report a family history of mental illness, which could be a contributing factor to their own mental health experiences and awareness.

---

### 8. Age vs. Work Interference, Colored by Treatment

A scatter plot that explores the relationship between age and how often mental health interferes with work, with points colored based on whether the individual sought treatment. Jitter has been applied to better visualize overlapping points.

![Age vs. Work Interference](images/age_vs_work_interfere.png)
*(Please replace this placeholder with your actual plot image: `age_vs_work_interfere.png`)*

> **Insight:** There isn't a strong linear relationship between age and work interference. However, across various interference levels, individuals who sought treatment are present in different age groups, suggesting that work interference prompts help-seeking behavior regardless of age.

---

### 9. Number of Survey Responses Over Time

This line chart shows the volume of survey responses collected over time, indicating the period of peak survey activity.

![Responses Over Time](images/responses_over_time.png)
*(Please replace this placeholder with your actual plot image: `responses_over_time.png`)*

> **Insight:** The survey collected responses primarily during a specific period in late 2014 to early 2015, with a peak in late August/early September 2014, reflecting focused data collection over a limited timeframe.

---

### 10. Proportion of Treatment Seekers Over Time

This line chart tracks the proportion of respondents seeking mental health treatment over the survey period.

![Treatment Trends Over Time](images/treatment_trends_over_time.png)
*(Please replace this placeholder with your actual plot image: `treatment_trends_over_time.png`)*

> **Insight:** The proportion of individuals seeking treatment remained relatively stable throughout the survey period, or showed slight fluctuations, indicating consistent reporting patterns regarding help-seeking behaviors.

---

## Key Findings and Insights

* **Gender Disparity in Responses:** The survey data is heavily skewed towards male respondents, which might affect the generalizability of findings to other genders.
* **Impact of Benefits:** The availability of mental health benefits appears to positively correlate with individuals seeking professional treatment.
* **Work Interference is Common:** Many respondents experience mental health interfering with work, prompting a need for supportive workplaces.
* **Age Distribution:** The tech workforce surveyed is predominantly young to middle-aged.
* **Temporal Consistency:** The patterns of responses and treatment-seeking behavior remained relatively consistent over the survey's collection period.

## Contact

Feel free to reach out if you have any questions or feedback!

### Zack Jones
* **Email:** zackjones.dataanalyst@gmail.com
* **LinkedIn:** www.linkedin.com/in/zjaytech/
