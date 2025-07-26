# Mental Health in Tech Survey Analysis

This project explores mental health trends in the tech industry using the [OSMI Mental Health in Tech Survey](https://www.kaggle.com/datasets/osmi/mental-health-in-tech-survey). Built with **R** and **ggplot2**, the analysis uses real-world survey data to visualize patterns related to mental health conditions, treatment, workplace support, and more.

---

## Dataset

- **Source**: [Open Sourcing Mental Illness (OSMI)](https://osmihelp.org/research)
- **File**: `survey.csv`
- **Attributes**: Includes demographics, treatment history, employer attitudes, and workplace support structures.

---

## Visualization 1: Comparative Analysis with Grouped Bar Chart

> *This visualization shows how respondents from the tech industry reported seeking mental health treatment, grouped by gender. It helps identify whether there's a noticeable difference in treatment-seeking behavior between genders.*

### Code:
```r
# STEP 1: Load required libraries
library(tidyverse)  # For data manipulation and plotting
library(readr)      # For reading CSV files
library(janitor)    # For cleaning column names

# STEP 2: Load the dataset (adjust path if needed)
survey <- read_csv("survey.csv") %>%
  clean_names()  # Converts column names to snake_case

# STEP 3: Simplify gender values to "Male" and "Female"
survey <- survey %>%
  mutate(gender = case_when(
    str_detect(str_to_lower(gender), "female|f") ~ "Female",
    str_detect(str_to_lower(gender), "male|m") ~ "Male",
    TRUE ~ "Other"
  ))

# STEP 4: Filter only "Male" and "Female" for the grouped chart
filtered_data <- survey %>%
  filter(gender %in% c("Male", "Female"))

# STEP 5: Group data by gender and treatment response
grouped_data <- filtered_data %>%
  group_by(gender, treatment) %>%
  summarise(count = n(), .groups = "drop")

# STEP 6: Create grouped bar chart
ggplot(grouped_data, aes(x = gender, y = count, fill = treatment)) +
  geom_col(position = "dodge") +
  labs(
    title = "Mental Health Treatment by Gender in Tech",
    x = "Gender",
    y = "Number of Respondents",
    fill = "Sought Treatment"
  ) +
  scale_fill_manual(
    values = c("Yes" = "#5ead6a",  # medium green
               "No" = "#d46c55")   # medium red
  ) +
  theme_minimal(base_size = 13) +
  theme(
    panel.background = element_rect(fill = "white", color = NA),
    plot.background = element_rect(fill = "white", color = NA)
  )
```
### Visualization

![image_alt](https://github.com/zJayTech/Mental-Health-in-Tech-Survey-Analysis/blob/main/treatment-by-gender.png?raw=true)

---
