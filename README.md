# Predicting-Asset-Intensity-with-Text-Analysis-BERT

This project investigates the feasibility of using text analysis with BERT (Bidirectional Encoder Representations from Transformers) to predict a company's asset intensity based on its textual descriptions.

**Data Preparation:**
* The project combines features (text descriptions) with labels (financial ratios like debt-to-equity, price-to-sales, return-on-assets).
Data cleaning steps include:
* Merging and cleaning the data.
* Removing outliers.
* Creating a binary variable for high debt-to-equity ratio.
* Tokenizing the descriptions (breaking text into smaller units).
* Removing unusual characters and very long descriptions.

**Text Analysis with BERT:**
* A pre-trained BERT model is used to process the textual descriptions. BERT helps understand the context and meaning within the text.
* The descriptions are tokenized and padded to ensure consistent size for model input.

**Logistic Regression Models:**
The project builds separate logistic regression models for each financial ratio:
* Debt-to-equity ratio - Achieved the highest accuracy (around 88.7%)
* Price-to-sales ratio - Performed better than random guess (around 66.9% accuracy) but has room for improvement.
* Return-on-assets ratio - Similar performance to price-to-sales ratio (around 74.9% accuracy).
A dummy classifier (predicting the majority class) is used as a baseline for comparison.

**Key Points:**
* The model using BERT outperforms a random guess in predicting all three financial ratios based on textual descriptions.
* Debt-to-equity ratio prediction achieved the highest accuracy, suggesting a stronger relationship between text and this ratio.
* Price-to-sales and return-on-assets models have room for improvement, indicating that text descriptions might not be the strongest indicator for these ratios.

Overall, this project demonstrates the potential of using BERT for text analysis to predict a company's financial health based on textual descriptions, although other factors likely play a significant role.
