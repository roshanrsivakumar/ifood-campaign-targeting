# ifood-campaign-targeting
RoshanRSivakumar | iFood marketing analytics: customer segmentation (KMeans) + campaign response prediction (LogReg, Random Forest) with targeting list, lift, and executive insights.
# iFood Marketing Analytics  
Customer Segmentation and Campaign Targeting

Built by RoshanRSivakumar

## Why this project exists
Marketing is art, but it still needs numbers that speak.  
This project builds a simple end to end targeting engine to answer one question:

**_Who is most likely to respond to a marketing campaign, and how do we prioritize them?_**

## What I built
1. Exploratory analysis to understand response patterns using income, recency, and spend
2. Feature engineering for marketing behavior
   1. TotalPurchases
   2. DealShare
   3. TotalKids
   4. Channel mix shares
3. Customer segmentation using KMeans
4. Campaign response prediction using
   1. Logistic Regression baseline
   2. Random Forest for stronger ranking
5. Targeting output
   1. Top 200 customers ranked by predicted response probability

## Key results from my run
1. Logistic Regression AUC: 0.8657  
2. Random Forest AUC: 0.8869  
3. Overall response rate: 0.1504  
4. Top 10 percent response rate: 0.6545  
5. Lift in top decile: 4.35  

These numbers show the model can rank audiences well, which is the real job of targeting.
