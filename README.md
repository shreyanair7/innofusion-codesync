# Mobile Health App Analysis – Compliance, Usability & Adoption

## Overview
This project analyzes mobile health applications to understand how regulatory compliance, usability, engagement, and communication features impact user trust, ratings, and adoption.

---

## Objectives
The project aims to:
- Understand variables related to compliance, engagement, communication, and usability
- Prepare and clean structured mobile health app review data
- Perform exploratory data analysis to identify meaningful trends
- Apply machine learning to predict high-performing apps
- Generate actionable recommendations for improving user trust and market success

---

## Dataset
The dataset contains survey-based evaluations of mobile health applications, including:
- Regulatory and privacy compliance indicators
- Usability and confidence-related responses
- Engagement and communication features
- Platform-specific ratings and adoption metrics

Due to the survey-driven nature of the data, several variables exhibit structured missing values and discrete responses.

---

## Data Preparation and Feature Engineering
Key preprocessing steps included:
- Handling structured missing values without dropping records
- Converting platform-specific ratings into numeric format
- Creating a unified `OverallRating` from iOS and Android ratings
- Engineering a composite `UsabilityScore`
- Encoding compliance, engagement, and communication features
- Creating a binary `HighRating` target variable for classification

Only cleaned and analytically reliable features were used for modeling and visualization.

---

## Exploratory Data Analysis
EDA focused on aggregated and frequency-based visualizations to account for discrete survey variables and limited variance.

Key findings from EDA include:
- App store ratings are highly concentrated between 4.0 and 5.0
- Social proof, measured through number of ratings and downloads, strongly influences success
- Usability and recommendation likelihood align closely with higher ratings
- Engagement and educational features appear more frequently in high-rated apps
- Clinical branding alone does not guarantee higher ratings

---

## Machine Learning Approach
Initial regression modeling performed poorly due to limited rating variance.  
The task was reframed as a classification problem to predict whether an app achieves a high rating (4.5 or above).

A Random Forest classifier was trained using an 80–20 train-test split, with feature importance analysis used to interpret model behavior.

---

## Key Model Insights
The most influential predictors of high app ratings were:
- Number of ratings and adoption signals
- Recommendation likelihood
- Engagement and educational features
- Pricing and monetization structure

These results highlight that usability, engagement, and visibility matter more than clinical branding alone.

---

## Strategic Recommendations
Based on the analysis:
- Improve usability and interface simplicity
- Encourage user reviews to build social proof
- Incorporate educational and goal-oriented engagement features
- Maintain transparent privacy and compliance practices
- Apply monetization strategies carefully to avoid trust erosion

---

## Technologies Used
Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Google Colab

---

## Conclusion
This project demonstrates that market success in mobile health applications is driven primarily by usability, engagement, and social proof rather than clinical branding alone.  
Data-driven analysis provides clear guidance for designing more trusted, effective, and successful digital health apps.

