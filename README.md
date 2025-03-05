# Customer Churn Prediction & Analysis

## Project Overview
Customer churn is a significant challenge in the finance sector, where businesses aim to retain customers and minimize attrition. This project leverages machine learning techniques to predict customer churn and analyze key factors contributing to it. We also use Power BI for visualization to present insights effectively.

## Dataset
- **Source**: eFinance Dataset
- **Total Records**: 10,000 (subset used: 2,000)
- **Features**:
  - `customer_id`: Unique identifier for each customer
  - `credit_score`: Creditworthiness of the customer
  - `country`: Customer’s country of residence
  - `gender`: Male/Female
  - `age`: Customer's age
  - `tenure`: Duration of relationship with the company
  - `balance`: Account balance
  - `products_number`: Number of products used
  - `credit_card`: If the customer has a credit card (1 = Yes, 0 = No)
  - `active_member`: If the customer is an active member (1 = Yes, 0 = No)
  - `estimated_salary`: Approximate income
  - `churn`: Target variable (1 = Churned, 0 = Retained)

## Tools & Technologies Used
- **Python**: Data preprocessing, feature engineering, and machine learning models
- **SQL (MySQL)**: Data extraction and cleaning
- **Machine Learning**: Logistic Regression, Random Forest, XGBoost
- **Power BI**: Data visualization and insights
- **GitHub**: Version control and project management

## Project Workflow
### Step 1: Data Preprocessing
- Checked for missing values (none found)
- Converted categorical variables (`gender`, `country`) into numerical format
- Standardized numerical features (`credit_score`, `balance`, `estimated_salary`)

### Step 2: Exploratory Data Analysis (EDA)
- **Churn by Gender**: Females had a slightly higher churn rate
- **Churn by Age**: Higher churn rate observed among younger customers
- **Churn by Country**: Varying churn patterns, with some regions showing significantly higher churn rates

### Step 3: Model Training & Evaluation
| Model                  | Accuracy | Precision (Churn) | Recall (Churn) | F1-Score (Churn) |
|------------------------|----------|------------------|---------------|----------------|
| Logistic Regression    | 0.82     | 0.60             | 0.18          | 0.28           |
| Balanced Logistic Reg  | 0.71     | 0.37             | 0.68          | 0.48           |
| Random Forest         | 0.86     | 0.74             | 0.47          | 0.57           |
| Tuned Random Forest   | 0.87     | 0.78             | 0.45          | 0.57           |
| XGBoost               | 0.86     | 0.71             | 0.52          | 0.60           |

### Step 4: Power BI Visualizations
- **Churn Rate (KPI Card)**
- **Churn by Gender (Bar Chart)**
- **Churn by Age Group (Column Chart)**
- **Churn by Country (Pie Chart)**

## Key Findings & Business Insights
1. **Age & Churn**: Younger customers are more likely to churn, suggesting the need for better engagement strategies for this segment.
2. **Gender & Churn**: Female customers showed a slightly higher churn rate.
3. **Country & Churn**: Some regions had a significantly higher churn rate, indicating location-based factors.
4. **Credit Score & Churn**: Customers with lower credit scores were more prone to churn.
5. **Active Members**: Retention was higher among active members.

## Recommendations
1. **Targeted Retention Programs**: Focus on high-risk customers (low credit score, young age group, inactive members).
2. **Improve Customer Engagement**: Personalized offers and loyalty programs for young customers.
3. **Regional Strategy**: Address region-specific churn trends by understanding local issues.
4. **Encourage Active Membership**: Increase benefits for active members to enhance retention.

## Conclusion
This project successfully identifies key factors influencing customer churn and provides actionable insights to improve customer retention. The combination of machine learning and Power BI makes the analysis both predictive and visually interpretable.

**Next Steps**: Deploy the model as a web app to predict churn in real-time.

## Author
**Aditya Sajith**

If you found this helpful, star the repository and share feedback.

