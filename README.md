# Udacity_Hypothesis_Testing
my final project of "Hypothesis Testing" course in Udacity


# A/B Testing Project — New vs. Old Landing Page

📌 #Overview 

- This repository contains my course project completed as part of the Udacity "Hypothesis Testing" course.

- The goal of the project is to determine whether introducing a new landing page increases conversion rates compared to the existing (old) page. Using real experiment data, I apply both frequentist hypothesis testing and logistic regression to evaluate the results.

📂 # Dataset

- ab_data.csv: Contains user visits, assigned group (control/treatment), landing page, and conversion outcome.
- countries.csv: Maps users to their country of origin (CA, US, UK).

🧪 # Methodology
**Part I — Probability & Sampling**

- Cleaned and explored the data (ensured group/page consistency).
- Calculated baseline conversion probabilities.

**Part II — Hypothesis Testing**

- Null Hypothesis (H₀): Conversion rates of old and new pages are equal.

- Alternative Hypothesis (H₁): Conversion rates differ.

**Methods used:**

- Bootstrapping & simulation (p_diffs > obs_diff)

- Two-sided Z-test for proportions

- Result: Fail to reject H₀. No significant difference between old and new pages.

**Part III — Regression Approach**

- Fit a logistic regression model predicting conversion based on page type.

- Extended model by adding country dummies (Canada as the baseline).

**Result:**

- ab_page coefficient not significant.

- Country had no meaningful effect (though UK showed a weak positive trend).

- Model fit was very poor (Pseudo R² ≈ 0).

📊 # Key Findings

- The new landing page does not increase conversion compared to the old page.

- Country of user does not significantly affect conversion likelihood.

- Both A/B test and regression agree — we fail to reject the null hypothesis.

⚙️ #Tech Stack

- Python: Pandas, NumPy, Matplotlib, Statsmodels, Scipy

- Statistical Methods: Hypothesis testing, bootstrapping, logistic regression

🚀 #How to Run

- Clone this repo:

git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>


- Install dependencies:

pip install -r requirements.txt


- Run the notebook:

jupyter notebook ab_test_analysis.ipynb

📖 #Interpretation

- Neither the A/B test nor the regression model found statistical evidence that the new page outperforms the old page.

- Recommendation: Stick with the old landing page, or test a different design.

📝 # Files in Repo

- ab_data.csv — Experiment dataset

- countries.csv — User-country mapping

- ab_test_analysis.ipynb — Main Jupyter Notebook

- README.md — Project documentation

👤 **Author**

Leila Soltani — [LinkedIn](https://www.linkedin.com/in/leilak-soltan/) | [GitHub](https://github.com/leilaksol)

