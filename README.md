# Brief Overview:  

This report tackles three key goals: 
1.	Predicting Customer Outreach Channels: We plan to create a model to forecast how likely each customer is to use Phone, WhatsApp, or Chatbot for their next contact within 90 days. This will help us guess customer likes and make channel management better. 
2.	Boosting Customer Satisfaction: To make service better, we will check and improve how happy customers are using main measures like Query Resolution Time (QRT), Resolution Accuracy (RA), Channel Efficiency (CE), Issue Impact Score (IIS). These measures will show us how to make service and customer experience better. 
3.	Finding Business Chances: We will look at customer info to spot ways to get new customers and give more loans to current ones. This means finding possible new customers and seeing patterns in current customers that show they might need more money products.
# A.  Prediction - 
# Modelling Approach:
Our modelling approach includes a complete process to make sure our predictions are accurate and effective:
1.	Data Cleaning and Exploration: We started by looking at the data to clean it up. We fixed missing values, dealt with outliers, got rid of duplicates, and made sure the data was good. This gave us a solid dataset to work with.
2.	Feature Correlation Analysis: Next, we looked at how different features relate to each other. This helped us understand which features matter most and reduce overlap, which made our model inputs better.
3.	Model Development: With our improved dataset, we built a Random Forest Classifier. We picked this method because it works well with big datasets and can spot complex patterns.
4.	Training and Evaluation: We split the dataset using 80% to train the model and 20% to test it. We trained the model on one part and checked how well it did on the other. This showed us how accurate and reliable the model is.
This step-by-step approach makes sure our predictive model is trustworthy and useful giving us good insights into what customers prefer for outreach.
# Expected benefit (value):
The solution offers several advantages:
1.	Customer Engagement That's Ahead of the Game: Predicting the chance of questions allows customer service teams   to reach out to customers before they ask, which boosts satisfaction and keeps customers around longer.
2.	Making the Most of Resources: Being able to guess when questions will come in helps teams use their people and time better. This means they can focus on customers who need help the most making the whole operation run smoother.
3.	More Money Coming In: Quick follow-ups can open doors to sell more products or different ones to customers, which might bring in extra cash.
# Algorithm Used:
The Random Forest Classifier was selected due to its robustness in handling a variety of data types and its ability to model complex interactions between features. It is particularly suitable for our case due to its ability to handle large datasets and provide interpretable results through feature.
1.	Hyperparameters: The model was trained using 100 trees (n_estimators=100) with a random state for reproducibility (random_state=42).
2.	Feature Scaling: Standard scaling was applied to ensure that all features contributed equally to the model's decision-making process.
# Final Evaluation Metrics:		
The model's performance was evaluated using the following metrics:
Accuracy of our model: 87%
                  
We have selected window for prediction is taken as 90 days, as it gives us the best balance between precision and recall, ensuring timely follow-ups without overwhelming the customer service team with false positives.
# B. Maximize Customer Satisfaction-
Key Metrics
1. Model Accuracy: With an accuracy of 0.87, the model predicts customer needs effectively, leading to faster and more accurate query resolutions.
2. Channel Usage: Channel 1 (WhatsApp channel as per given file) is the most preferred by customers. Ensuring its efficiency is crucial for maintaining high satisfaction levels.
3. Major Issues: Enquiries and Login are the most frequent issue. Addressing these effectively will significantly enhance customer experience.
Quantifying the Customer Satisfaction
1. Query Resolution Time (QRT): Average time to resolve queries. Current QRT is: 83 days; Target: < 60 days to get maximize satisfaction.
2. Resolution Accuracy (RA): With 87% accuracy, we aim for correct resolutions. Target: > 90%.
3. Channel Efficiency (CE): Currently 61.7% customers prefer Channel 1 for communicating their problems followed by Channel 2 and followed by Channel 0.
4. Issue Impact Score (IIS): Frequency and severity of Enquiries and Login issues are too high. This can be managed through proper communication with the help desk and usage of AI communicating techniques.
Benefits of quantification
1. Improved Response Time: Reducing QRT will enhance satisfaction.
2. Optimized Channel Performance: Increasing CE for Channel 1 will reinforce customer trust.
3. Targeted Issue Resolution: Prioritizing enquiry issues with new customers (here new customers are people with 0-5 months of joining to our company) and improving login techniques and framework will directly boost our customer satisfaction.
# C. Business Opportunities -

1. Targeting different segments: As from the data analysis done to the given csv file, we can see that we can categorize the customers based on their CIBIL Score Band (cbs_band) and their time as a TVS Credit Customer (MOB_DIFF).
2. Referral Programs: Implement referral incentives to leverage existing satisfied customers in acquiring new clients.
3. Credit Analysis of Customers: Analysing the existing customers credit profiles to identify those eligible for additional loans. 
4. Personalizing Loan Offers: We would customize loan offers based on customer’s financial behaviour and repayment history.
5. Campaign through Channels: Notify the customers about any campaigns through most preferred channel (here in our case is ‘WhatsApp’).
