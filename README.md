# Credit Risk Data Analysis

This repository contains an exploratory data analysis (EDA) of the German Credit Risk dataset. The primary focus is to investigate the relationship between housing status and the amount of credit requested by borrowers. This analysis provides insights into how different housing statuses (free, own, rent) may influence the credit needs of applicants, which can be valuable for financial institutions in assessing credit risk and tailoring financial products.

## Table of Contents

1. [Project Overview](#project-overview)
2. [Research Question](#research-question)
3. [Data Description](#data-description)
4. [Analysis](#analysis)
5. [Key Insights](#key-insights)
6. [Conclusion](#conclusion)
7. [Future Work](#future-work)
8. [Contributing](#contributing)
9. [License](#license)

## Project Overview

The aim of this project is to explore the relationship between housing status and the amount of credit requested by applicants. By analyzing the dataset, we can uncover patterns and provide insights into how housing conditions impact borrowing behavior and risk levels among different borrower groups.

## Research Question

**How does housing status (free, own, rent) affect the amount of credit requested by applicants?**

Understanding this relationship can help lenders better assess creditworthiness and design products that cater to different housing groups.

## Data Description

The dataset used for this analysis includes the following key features:

- **Housing Status**: Indicates whether the applicant's housing is free, owned, or rented.
- **Credit Amount**: The total amount of credit requested by the applicant.
- **Other Features**: Purpose of the loan, account balances, and other demographic details.

### Handling Missing Values

- Variables of interest (Housing and Credit Amount) had no missing values, so no rows were dropped.
- Variables like "Saving Account" and "Checking Account" had missing values but were not removed to avoid biasing the dataset, as they impacted 394 out of 1000 observations.

## Analysis

1. **Exploratory Data Analysis (EDA)**:
   - Visualized the distribution of credit amounts across different housing statuses using violin plots.
   - Calculated summary statistics (mean, median, standard deviation) for credit amounts based on housing status.

2. **Insights from Housing Status**:
   - Applicants with "free" housing request higher and more varied credit amounts compared to those who own or rent, possibly due to lower living expenses and greater disposable income.

3. **Grouping and Data Considerations**:
   - Uncommon categories in the "Purpose" variable were grouped under a broader category called "Other" to ensure more balanced representation and clarity in analysis.

## Key Insights

- **Higher Credit Requests for Free Housing**: Applicants in free housing have a higher mean credit request (4906) compared to those who own (3061) or rent (3123).
- **Implication of Free Housing**: Free housing may indicate various scenarios such as living with family, employer-provided housing, or government assistance, potentially leading to increased borrowing for significant expenses or investments.
- **Purpose and Frequency**: Less frequent purposes like "repairs" or "vacation" were grouped into an "Other" category to avoid skewed results due to their low representation in the dataset.

## Conclusion

The analysis indicates a strong relationship between housing status and the amount of credit requested. Applicants with free housing generally request higher credit amounts, suggesting different financial behaviors and needs. However, this analysis is limited by the absence of other relevant financial variables like income or employment status, which could provide additional context.

## Future Work

- **Incorporate More Financial Variables**: Future analyses could include additional financial variables such as income, employment status, or credit history for a more comprehensive understanding.
- **Predictive Modeling**: Implementing predictive models to assess the likelihood of loan approval or default based on housing status and other financial indicators.
- **Tool Development**: Creating a tool using predictive modeling to assess credit approval likelihood based on financial indicators.

## Contributing

Contributions are welcome! If you have suggestions for improvements or new insights, feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## How to View the Analysis

To view the complete analysis, refer to the [Jupyter Notebook](Credit%20Risk%20Data%20Analysis.ipynb) file in this repository.
