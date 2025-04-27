# Home Credit Default Risk Analysis

This repository contains the results of an analytical project that follows the CRISP-DM methodology to analyze the Home Credit Default Risk dataset from Kaggle.

---

### Methodology

We adhere to the CRISP-DM (Cross-Industry Standard Process for Data Mining) framework, which consists of the following phases:

1. **Business Understanding**: Grasping the project's objectives and requirements from a business perspective.
2. **Data Understanding**: Collecting and familiarizing ourselves with the data to identify quality issues and gain initial insights.
3. **Data Preparation**: Cleaning and transforming the data to create a suitable dataset for modeling.
4. **Modeling**: Applying various modeling techniques to the prepared data to develop predictive models.
5. **Evaluation**: Assessing the models to ensure they meet business objectives and selecting the best-performing one.
6. **Deployment**: Implementing the selected model into a real-world application for practical use.

---

### Data Source

The dataset used in this project is sourced from the Home Credit Default Risk competition on Kaggle. It comprises extensive information on loan applicants, including demographic details, financial status, and past loan records.

---

### Business Problem

The primary challenge faced by the loan applicant selection and processing teams is the difficulty in assessing the repayment capability of unbanked and underserved populations. These individuals often encounter significant barriers to obtaining financial loans due to their limited or nonexistent credit histories. This creates a pressing need to accurately quantify the risk of loan defaults to facilitate more inclusive financial decision-making. The lack of precise risk assessments can lead to either penalizing viable applicants or granting loans to individuals with high default probabilities, which ultimately affects both the organization's financial health and its ability to serve underserved communities. Metrics such as applicant acceptance rates, repayment rates, and overall portfolio health will highlight the severity of this issue.

---

### Potential Solution

The goal of this project is to predict the likelihood of an applicant defaulting on a loan. By leveraging various data sources, including behavioral and transactional information, we aim to build one or more predictive models to assess each applicant's repayment capability. This analysis will assist in making informed credit decisions and managing potential risks.

---

### Business Value

The primary business value of this project is the ability to predict the likelihood of loan default, which is essential for financial institutions in minimizing credit risk and improving their lending strategies. By accurately assessing the risk of individual applicants, the model helps in making data-driven decisions regarding loan approvals, interest rates, and credit limits.

This analysis can lead to:
- **Reduced Default Rates**: By identifying high-risk applicants early, banks and lending institutions can take preventive measures, such as offering alternative terms or denying high-risk loans.
- **Increased Operational Efficiency**: Automating the decision-making process with a predictive model reduces the time and effort required for manual risk assessments.
- **Improved Customer Experience**: By optimizing loan offerings based on predicted risk, financial institutions can tailor their services, ensuring that applicants are more likely to receive loans suited to their financial situations.
- **Regulatory Compliance**: Proper risk management and accurate credit assessments help financial institutions comply with regulatory requirements regarding lending practices and risk exposure.
- **Enhanced Marketing and Sales**: Beyond risk management, the provided data offers valuable insights into customer demographics, behavior, and financial history. This information can be leveraged by marketing and sales teams to better target potential customers, personalize product offerings, and identify profitable market segments.

Ultimately, this project contributes to better financial decision-making, risk management, and business growth, leading to higher profitability and sustainability for lending institutions.

---

### Personal Contribution

The content of this repository will differ from the group assignment developed separately. In that protion of the project, I played a facilitator role, contributing by compiling, expanding, and cleaning our group’s models, as well as leading the development of the presentation. Although my personal exploratory data analysis (EDA) was delayed, this gave me the opportunity to take a deeper dive into the data beyond the initial group-level analysis. As a result, this repository will reflect more comprehensive insights derived from a more thorough analysis than was performed in the group portion of this project. Additionally, I will be able to work on segmenting the data to train independent models that will be able to better predict default rate for the independent segments.

---

### Project Difficulties

Throughout this project, several challenges arose. First, the datasets were large and comprised multiple CSV files, which made feature engineering particularly difficult. Identifying potentially useful features required a thorough review of numerous columns across each CSV to assess their relevance for creating beneficial aggregated metrics. Additionally, the large volume of records resulted in slow processing times, sometimes causing the RStudio environment to crash when running the code to evaluate our work. To address this, we optimized memory usage by ensuring that large datasets were first aggregated, merged into the main dataset, and then removed and garbage collected for each of the side tables. This approach helped maintain the efficiency of the environment and allowed us to continue working with the large data without memory issues. Finally, the dataset exhibited a significant class imbalance, which required careful adjustments to ensure accurate modeling. Given the large number of records, we chose to undersample the majority class, as this approach was unlikely to compromise the accuracy of the model while addressing the imbalance.

---

### Learning Outcomes

This analytics project played a significant role in enhancing our understanding of data analytics. It provided valuable experience in cleaning datasets, mining data for insights, and visualizing the results. The CRISP-DM framework was particularly useful, allowing us to efficiently progress through each stage of the project and reinforcing the importance of a production-grade methodology. Additionally, the project fostered team cooperation, enabling us to strengthen our communication skills while working collaboratively. On a personal level, this project allowed me to create my first analytics portfolio—a long-awaited milestone, especially considering my background in software development—and to continue refining the statistical skills I aim to master.

---

### Acknowledgments

This project is a part of the coursework for the Master of Science in Business Analytics (MSBA) program at the University of Utah. We extend our gratitude to the University of Utah for providing the academic foundation and resources to pursue this analysis. Additionally, we thank Kaggle and Home Credit Group for providing the dataset and hosting the competition.
