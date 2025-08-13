# FinalCapstone
The goal of this project is to perform sentiment analysis on Yelp reviews dataset, specifically to determine if a given review opinion is “positive”, “negative”, or “neutral”.

The Yelp reviews dataset consists of reviews of businesses scraped from 2015 and developed for the Yelp Dataset Challenge. 
http://www.yelp.com/dataset_challenge

The dataset is sourced from hugging face.
https://huggingface.co/datasets/Yelp/yelp_review_full

The dataset consists of two .csv files: training.csv with 650k records and test.csv. with 50k records. Text preprocessing for both datasets takes nearly an hour. To prevent having to regenerate the dataset, the dataframe was written to a local binary file (pickled). However, due to size constraints, the .csv and .pkl files are not able to be included in this repository. The .csv files must be present in the repository to run the notebooks. 

Logistic regression, SVM, Naïve Bayes, and Random Forest machine learning models were created to perform multinomial classification. Additionally, a VADER pre-trained model was used as an “automatic” sentiment analyzer to compare against the classifier models. A comparison of the results was performed to show that logistic regression classification model performed the best outcome with an accuracy of nearly 70%.
