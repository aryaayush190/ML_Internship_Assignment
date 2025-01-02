# Machine Learning Assignment: User Churn Prediction

## Objective
The goal of this assignment is to predict which users are most likely to churn (i.e., stop returning or purchasing) based on their behavior on an e-commerce platform. Additionally, the project aims to provide actionable insights into the reasons behind churn and suggest strategies for improving user retention.

---

## Dataset
The dataset, `events.csv`, contains user activities on the platform, including:
- **Event types**: `view`, `cart`, `purchase`
- **Timestamps** for events
- **User identifiers**
- **Monetary values** (where applicable)

---

## Deliverables
### 1. Exploratory Data Analysis (EDA)
- Overview of the dataset and user behavior.
- Key insights:
  - Distribution of events over time.
  - Popularity of categories and brands.
  - User-level metrics like total spend and visit frequency.

### 2. Churn Definition
- Defined churn as no user activity for more than **30 days**.
- Justification: Aligns with industry benchmarks and highlights inactive users.

### 3. Feature Engineering
- User-level features:
  - **RFM Metrics**: Recency, Frequency, and Monetary values.
  - **Session-Based Metrics**: Session count, average session duration.
  - **Behavioral Patterns**: View-to-cart and cart-to-purchase ratios.
  - **Category Preferences**: Most viewed/purchased categories.

### 4. Predictive Modeling
- **Model**: Random Forest Classifier.
- **Evaluation Metrics**:
  - Precision, Recall, F1 Score.
  - AUC for classification performance.

### 5. Interpretability
- Feature importance analysis.
- Insights from SHAP values.

### 6. Business Recommendations
- Re-engage users with high Recency values via targeted campaigns.
- Encourage purchases from users with moderate Frequency and Monetary values.
- Focus retention efforts on categories with higher churn risk.
- Implement loyalty programs and personalized offers.

---

## Project Structure
```
├── data/
│   └── events.csv           # Dataset
├── notebook/
│   └── ML_Assignment.ipynb  # Main notebook for analysis
├── README.md                # Project overview
└── requirements.txt         # Required Python libraries
```

---

## Requirements
Install the required Python libraries:
```bash
pip install -r requirements.txt
```

---

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/username/ml-assignment.git
   cd ml-assignment
   ```
2. Open the notebook:
   ```bash
   jupyter notebook notebook/ML_Assignment.ipynb
   ```
3. Run all cells to reproduce the analysis and results.

---

## Evaluation Criteria
1. **Model Metrics (40%)**: Evaluation using precision, recall, F1 score, and AUC.
2. **Problem-Solving Approach (20%)**: Clear problem definition and solution strategy.
3. **Feature Engineering (20%)**: Relevance and creativity of features.
4. **Code Quality & Documentation (10%)**: Well-structured, commented, and reproducible code.
5. **Reference Research Utilization (10%)**: Effective use of the provided research paper.

---

## Business Insights & Recommendations
- **Target high Recency users** with personalized offers to encourage re-engagement.
- **Boost Frequency and Monetary scores** with loyalty rewards.
- **Address churn in high-risk categories** through pricing optimization and bundling.

---

## References
- Research Paper: http://www.evaascarza.com/ascarza_et_al_choice_symposium.pdf

---

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.

