# iFood Marketing Analytics: Customer Segmentation and Campaign Targeting

**Author:** Roshan R Sivakumar (GitHub: roshanrsivakumar)  
**Portfolio:** https://www.roshanrsivakumar.com  
**Search keywords:** roshanrsivakumar, Roshan R Sivakumar, marketing analytics, campaign targeting, customer segmentation

## Overview
This project builds an end to end marketing analytics workflow to improve campaign efficiency. It combines customer segmentation and campaign response prediction to create a ranked targeting list of customers most likely to respond.

## Objectives
- Understand what drives campaign response using EDA
- Segment customers based on value and behavior
- Predict campaign response probability using machine learning
- Generate an actionable targeting list for campaign activation

## What I built
- **EDA and KPI insights** using Income, Recency, and Total Spend
- **Feature engineering** for marketing behavior:
  - `TotalPurchases`
  - `DealShare`
  - `TotalKids`
  - Channel mix shares (Web, Store, Catalog)
- **Customer segmentation** using **KMeans**
- **Response prediction** using:
  - Logistic Regression (baseline)
  - Random Forest (performance model)
- **Targeting deliverable**: Top 200 customers ranked by predicted response probability

## Key results (from my run)
- **Logistic Regression AUC:** 0.8657  
- **Random Forest AUC:** 0.8869  
- **Overall response rate:** 0.1504  
- **Top 10 percent response rate:** 0.6545  
- **Lift in top decile:** 4.35  

## How to run (Google Colab)
### Step 1: Place the dataset
Because datasets can be large or have licensing constraints, the raw dataset may not be committed to GitHub.

Create this path:
- `data/ifood_df.csv`

If you keep the CSV in Google Drive, update the `path` variable inside Notebook 01 accordingly.

### Step 2: Run notebooks in order
1. **01_data_check_and_eda.ipynb**
   - Loads data
   - Creates features
   - Generates EDA charts and insights
2. **02_segmentation.ipynb**
   - Fits KMeans segmentation
   - Exports segment profile and segmented dataset
3. **03_response_model_targeting.ipynb**
   - Trains Logistic Regression and Random Forest models
   - Evaluates AUC and lift
   - Exports targeting list and scored dataset

## Outputs (deliverables)
- Segment profile with response rate by segment
- Target list of top 200 customers ranked by predicted response probability
- Scored dataset with predicted probabilities for all customers

## Business recommendations
- Prioritize **high value and recent buyers** first for best ROI
- Run campaigns in **waves**:
  - Wave 1: Top ranked customers (highest predicted response)
  - Wave 2: Mid value customers with personalized recommendations
  - Wave 3: Deal sensitive customers using controlled discount tests
- Track performance weekly:
  - Response rate by segment
  - Response rate by decile of predicted probability
  - Lift over baseline targeting

## KPI glossary
Includes definitions for:
- Response rate
- Recency
- Total spend (`MntTotal`)
- Total purchases
- Deal share
- Campaign acceptance (`AcceptedCmpOverall`)
- Channel mix

## Screenshots
Includes EDA charts, segment profile visuals, model metrics, and targeting list previews.

## Topics (GitHub)
roshanrsivakumar, RoshanRSivakumar, marketing-analytics, customer-segmentation, campaign-targeting, response-modeling, machine-learning, python, kmeans, random-forest, logistic-regression, auc, lift, colab
