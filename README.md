# Valentine's Day Spending Behavior Analysis

## Project Overview
This project analyzes Valentine's Day spending patterns using survey data from the National Retail Federation. It explores which spending categories most influence overall spending and identifies spending behavior profiles across different age groups. The National Retail Federation (NRF) in the United States conducts annual surveys to explore consumer behavior around Valentine’s Day. For over a decade, these surveys have provided insights into how consumers celebrate Valentine's Day, including details about their spending habits across various categories. This project explores two datasets to answer key research questions related to Valentine's Day consumer spending behavior.  More information about the datasets can be found here: https://github.com/rfordatascience/tidytuesday/tree/main/data/2024/2024-02-13.

This analysis sheds light on the complexities of Valentine's Day spending behavior, providing actionable insights for businesses and marketers targeting consumers during this holiday. The primary goal of this project is to analyze historical data to answer the following research questions:

1. Which spending categories most strongly influence overall Valentine's Day spending patterns?

2. What distinct spending behavior profiles exist among people based on their spending categories, and how do these profiles correlate with age groups?

## Dataset Information
Two datasets are used in this analysis:

1. **Historical_spending**: This dataset contains numeric data representing the average percentage spent in each category: Candy, Flowers, Jewelry, Greeting Cards, Evening Out, Clothing, and Gift Cards.

2. **Gifts_age**: This dataset contains spending data categorized by age groups, with variables for Age, Candy, Flowers, Jewelry, Greeting Cards, Evening Out, Clothing, and Gift Cards. The gifts_age dataset divides Age into six groups for individuals aged 18 and older.

The data was sourced from the TidyTuesday repository.

## Approach
The analysis was conducted in R, and the following steps were taken:

1. *Descriptive Analysis*: I began with a descriptive analysis of both datasets using the summary function to better understand their structure and contents.

2. *Data Transformation*: The gifts_age dataset was transformed from a wide to a long format to facilitate analysis and visualization.

3. *Data Visualization*:
   
    a. I created bar and scatter plots to explore the gifts_age dataset. The bars represent the spending categories, while black dots indicate the overall average spending for each age group.

    b. To investigate the influence of different spending categories on overall spending patterns, I visualized the results of a Principal Component Analysis (PCA) with a rotation plot matrix. This allowed for an understanding of how each spending category contributes to overall spending behavior.

4. *Principal Component Analysis (PCA)*: For the first research question, I performed PCA on the historical_spending dataset to identify the spending categories that most strongly influence Valentine's Day spending patterns.

5. *Clustering Analysis*: To explore distinct spending behavior profiles based on spending categories and age groups, I applied a clustering algorithm. The process included the following steps:

    a. Created an elbow plot to determine the optimal number of clusters.
   
    b. Scaled the gifts_age dataset and applied PCA.
   
    c. Generated clusters based on the scaled and transformed data.
   
    d. Visualized the clusters and age groups in scatter plots for PC1 vs. PC2. The scatter plots display cluster colors to compare the distributions of spending profiles and their relationship to age groups.

## Key Findings
The analysis provides insights into:

1. Key spending categories that influence Valentine's Day spending patterns.

2. Distinct spending behavior profiles among different age groups.

These findings offer a clearer understanding of consumer spending behavior during Valentine's Day, helping to tailor marketing strategies and business decisions.

## Tools and Techniques
1. Programming Language: R

2. Libraries Used: ggplot2, dplyr, tidyverse, broom, patchwork

3. Analysis Techniques: Desriptive Analysis, Exploratory Data Analysis (EDA), Principal Component Analysis and K-means Clustering



## Future Work 
Further analysis could explore:

1. Additional demographic factors influencing spending behavior (e.g., income, location).

2. Trends in spending patterns over the years to identify shifts in consumer preferences.

## Contact
If you have questions or suggestions, feel free to reach out:

Author: Adeena Amersi

Email: adeenaamersi@gmail.com











