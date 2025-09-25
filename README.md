# Hotel Booking Cancellation Prediction

This project develops machine learning models to predict hotel booking cancellations using a dataset of 36,275 reservations from a Lisbon hotel (2017–2018).  
It was completed as a capstone project at the University of Pittsburgh.

## Project Overview
Hotel cancellations create financial losses and operational inefficiencies. Hotels often rely on overbooking, but this can backfire when more guests arrive than expected.  
This project explores a data-driven alternative: predicting which bookings are most at risk of cancellation and identifying the factors that drive those outcomes.

**Key questions:**
1. Can we predict how likely a booking is to be canceled?  
2. What factors most strongly influence cancellation risk?  

## Data
- 36,275 booking records from one hotel in Lisbon, 2017–2018  
- 16 features including:
  - Numeric: lead time, number of nights, average price per room  
  - Categorical: room type, market segment, meal plan, arrival month  
  - Behavioral: number of special requests, repeated guest, previous cancellations  

## Methods
- **Exploratory Data Analysis (EDA):** Distributions, transformations for skewed variables, categorical comparisons, class imbalance.  
- **Models:**
  - LASSO Logistic Regression – interpretable coefficients, built-in feature selection.  
  - Random Forest – ensemble model capturing nonlinear interactions, feature importance ranking.  
- **Threshold Tuning:** Adjusted cutoffs using F1 score and Youden’s Index to balance sensitivity vs specificity.  

## Results
- **Random Forest**: ~90% accuracy, balanced sensitivity and specificity.  
- **LASSO**: ~79% accuracy, highly interpretable coefficients.  
- **Key predictors**:  
  - Longer lead times and higher prices increase cancellation likelihood.  
  - More special requests and offline/corporate bookings reduce cancellation likelihood.  

## Business Impact
Predictive modeling enables hotels to:
- Adjust room pricing for high-risk bookings.  
- Send reminders or targeted offers to reduce cancellations.  
- Manage overbooking strategies more effectively.  

## Repository Structure
- `notebooks/` → Jupyter notebooks with EDA and modeling steps  
- `reports/` → Written report and presentation slides  
- `figs/` → Visualizations and model outputs  
- `src/` → Reusable code functions  

## Future Work
- Test additional models (XGBoost, LightGBM).  
- Add SHAP values for interpretability.  
- Extend dataset to multiple hotels or real-time data.  

## Author
Kerem Onipede  
Email: keremonipede@gmail.com

LinkedIn: [your-link-here]
