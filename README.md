# Home Credit Default Risk Analysis

This repository contains the results of an analytical project that follows the CRISP-DM methodology to analyze the Home Credit Default Risk dataset from Kaggle.

### Project Overview

The goal of this project is to predict the likelihood of an applicant defaulting on a loan. By leveraging various data sources, including behavioral and transactional information, we aim to build a predictive model that assesses each applicant's repayment capability. This analysis will assist in making informed credit decisions and managing potential risks.

### Methodology

We adhere to the CRISP-DM (Cross-Industry Standard Process for Data Mining) framework, which consists of the following phases:

1. Business Understanding: Grasping the project's objectives and requirements from a business perspective.
2. Data Understanding: Collecting and familiarizing ourselves with the data to identify quality issues and gain initial insights.
3. Data Preparation: Cleaning and transforming the data to create a suitable dataset for modeling.
4. Modeling: Applying various modeling techniques to the prepared data to develop predictive models.
5. Evaluation: Assessing the models to ensure they meet business objectives and selecting the best-performing one.
6. Deployment: Implementing the selected model into a real-world application for practical use.

### Data Source

The dataset used in this project is sourced from the Home Credit Default Risk competition on Kaggle. It comprises extensive information on loan applicants, including demographic details, financial status, and past loan records.

### Repository Structure

- `documents`: Contains initial planning and design artifacts. 
- `data/`: Contains the raw and processed datasets.
- `notebooks/`: Jupyter notebooks detailing the analysis and modeling processes.
- `models/`: Saved models and related artifacts.
- `reports/`: Generated reports and visualizations summarizing the findings.
- `src/`: Source code for data processing, modeling, and evaluation.

### Acknowledgments

This project is a part of the coursework for the Master of Science in Business Analytics (MSBA) program at the University of Utah. We extend our gratitude to the University of Utah for providing the academic foundation and resources to pursue this analysis. Additionally, we thank Kaggle and Home Credit Group for providing the dataset and hosting the competition.

# Repository Branch Strategy - WILL BE REVISED SOON -

#### 1. Main Branch (or main/master)

-   **Purpose:** This is the primary branch that always contains the production-ready code.
-   **Characteristics:**
    -   It should always be deployable.
    -   Bug fixes and updates from develop or hotfix branches are merged here after thorough testing.

#### 2. Develop Branch (develop)

-   **Purpose:** Acts as the integration branch for features and serves as a pre-production branch.
-   **Characteristics:**
    -   Developers merge their feature branches here.
    -   Used for testing and ensuring features work together before merging to main.
    -   Deployment to a staging environment often happens from this branch.

#### 3. Feature Branches (feature/feature-name)

-   **Purpose:** Created for individual features or tasks, allowing isolated development.
-   **Characteristics:**
    -   Branched off develop.
    -   Once the feature is complete and tested, it's merged back into develop.

#### 4. Hotfix Branches (hotfix/hotfix-name)

-   **Purpose:** Used to fix critical bugs in the production environment.
-   **Characteristics:**
    -   Branched off main.
    -   Changes are tested and merged into both main and develop to ensure consistency.

#### 5. Release Branches (release/release-name)

-   **Purpose:** Prepares a new production release.
-   **Characteristics:**
    -   Branched off develop once enough features are complete and ready for release.
    -   Bug fixes or minor tweaks can be made directly in this branch.
    -   Merged into both main (for deployment) and develop (to include any final fixes).

#### 6. Bugfix Branches (bugfix/bug-name)

-   **Purpose:** Addresses specific bugs identified during development or testing.
-   **Characteristics:**
    -   Branched off develop or sometimes a release branch.
    -   Merged back into the parent branch upon completion.
    -   Optional: Custom Branches

Depending on team size and workflow:

-   Experiment Branches: For trying out ideas that might not make it into production.
-   Testing Branches: For running isolated tests on specific environments.

Visual Workflow Example:

-   Main ↔ Develop ↔ (Feature/Release/Hotfix) ↔ Main
-   Ensure CI/CD pipelines are set to test, build, and deploy based on branch rules.
