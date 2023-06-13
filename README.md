# Sentimental-Analysis-of-Clothing-Reviews
Open Source Dataset used to Analyze Sentiments of Clothing Reviews Given By Customers. 

We intend to achieve our goals for this analysis by using various Machine learning
techniques (classification in tandem with natural language processing techniques at the
core) to efficiently process textual data in the form of reviews, further selecting the best
classification algorithms that successfully classify review sentiment along with a detailed
report based on sentiment analysis that can help the organization move forward with the
aid of data driven decision making.

# Data Description
A women's clothing e-commerce dataset centered on customer reviews is found here. Its
nine supportive elements provide an excellent setting for dissecting the text's various
dimensions. The data set includes 23486 Rows and 10 feature variables:
• Clothing ID: Integer Categorical variable referring to specific piece being reviewed.
• Age : Positive Integer variable of the reviewer’s age.
• Title: String variable for the title of the review.
• Review Text: String variable defining the review body.
• Rating: Positive Ordinal Integer variable for the product score granted by the
customer from 1 Worst to 5 Best.
• Recommended IND: A binary variable indicating if a customer recommends a
product where 1 indicates a recommendation and 0 indicates a disapproval
• Positive Feedback Count: Positive Integer documenting the number of other
customers who found this review positive.
• Division Name: Categorical name of the product high level division.

# Interesting Facts

After visualization and analysis, we could explore plentiful about the nature of our data,
relevant columns, categorical distributions, correlations etc. We have tried to summarize
the main points and our findings below. This will help us move forward when we reach
the model creation and evaluation stage.
• Approximately 3000 missing values are present which is only 1% of the data. We
took care of them by removing certain columns all together and by replacing
specific values
• ~50% of the positive feedback comes from the top 20% reviews
• 31 – 52-year-old people are 66.5% of the reviewers according to the data
distribution
• The dataset is highly imbalanced with 82% of values in the class of interest (1:
Recommended)
• According to the polarity calculations, most of the reviews are of neutral polarity
• The top 3 items received an average rating of ~4.2, and an average
recommendation rate of 83%. Furthermore, these products are normal sized
dresses as per label.
• Since most reviews are highly positive it will be a challenge to balance specificity
with high sensitivity.

# Results

Sr No         Model            Sensitivity     Specificity    ROC/AUC
1             KNN              98.2            66.8           0.85314
2             Naïve Bayes      93.1            89.1           0.96551
3             Gradient Boost   92.9            95.0           0.96961
4             Random Forrest   94.7            86.1           0.92582
5             Neural Network   96.2            56.9           0.81345
