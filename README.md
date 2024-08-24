# PFG-Bank-Data-Driven-Credit-Card-Design

### Project Description:
In this comprehensive case study, I worked on optimizing a direct mail credit card solicitation campaign for PFG Bank, focusing on maximizing profits through data-driven decision-making. The goal was to design and implement a strategy that efficiently targeted up to 750,000 prospects with one of twelve different product offers. The campaign's design was informed by uplift modeling and propensity modeling using Logistic Regression, Random Forest, and XGBoost algorithms. The project involved strategic customer segmentation, model training, evaluation, and interpretation to identify the most profitable segments for targeted solicitation.

### Technology Stack:
- **Data Handling and Analysis:** Python, pandas, pyrsm
- **Machine Learning Models:** Logistic Regression, Random Forest, XGBoost
- **Modeling Tools:** GridSearchCV for hyperparameter tuning, sklearn for machine learning pipelines
- **Visualization:** Matplotlib for performance visualization and comparison

### Key Accomplishments:

#### 1. **Data Preparation and Segmentation:**
   - Combined multiple datasets into a single stacked dataset for uplift analysis.
   - Created training and test splits using stratified sampling to ensure balanced representation of key variables.
   - Added new variables such as the treatment flag and computed uplift scores for each prospect based on the models.

#### 2. **Model Training and Tuning:**
   - **Logistic Regression:** Implemented logistic regression models to predict conversion probability for both control and treatment groups. Computed uplift scores by subtracting the control group's predicted probabilities from the treatment group's.
   - **Random Forest:** Trained and tuned Random Forest models using GridSearchCV, adjusting hyperparameters such as `n_estimators` and `max_features` to optimize model performance.
   - **XGBoost:** Employed XGBoost for gradient boosting, tuning parameters such as `max_depth`, `n_estimators`, and `subsample`. XGBoost provided the highest accuracy and uplift in the final results.

#### 3. **Performance Evaluation and Comparison:**
   - Evaluated models using metrics such as AUC, incremental uplift, and total incremental profit.
   - Compared the performance of uplift models and propensity models across different algorithms.
   - Visualized the results through incremental uplift plots and uplift bar charts, which helped in identifying the most responsive customer segments.

#### 4. **Profit Optimization:**
   - Calculated the incremental profits based on the uplift models and identified the optimal percentage of the population to target.
   - Demonstrated that targeting based on uplift models generally yielded higher profits than propensity models across all algorithms.
   - Used these findings to recommend targeting strategies that would maximize profits for PFG Bank.

### Key Outcomes:

#### **Optimized Targeting Strategy:**
   - **Logistic Regression:** Identified that targeting 20% of the customer base using the uplift model was optimal, resulting in a total incremental profit of approximately $6,658.
   - **Random Forest:** Suggested targeting 30% of the customer base with the Random Forest uplift model, yielding a total incremental profit of $6,444.
   - **XGBoost:** XGBoost uplift model proved to be the most effective, recommending targeting 30% of the customer base, which generated the highest incremental profit of approximately $12,132.

#### **Enhanced Model Performance:**
   - Successfully demonstrated the superior performance of uplift models over propensity models in terms of incremental profit.
   - The XGBoost uplift model outperformed both Logistic Regression and Random Forest, emphasizing the importance of advanced ensemble methods in predictive analytics.

#### **Actionable Insights:**
   - Provided clear recommendations on customer segmentation and targeting strategies that PFG Bank can implement to maximize the return on investment from their credit card solicitation campaigns.
   - The analysis highlighted the importance of focusing on the most responsive segments, avoiding segments where the campaign could have a negative impact.

### Conclusion:
This project showcases a sophisticated approach to optimizing marketing campaigns through uplift modeling and machine learning. By applying advanced techniques such as Random Forest and XGBoost, I was able to provide PFG Bank with actionable insights that directly impact their bottom line, demonstrating the power of data-driven decision-making in financial services.
