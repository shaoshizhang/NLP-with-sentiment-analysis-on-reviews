This project has three parts.

The first part is to scrape reviews from Trustpilot.com that the company has at least 500 reviews. The reviews are written to a CSV file with the following columns: companyName , datePublished , ratingValue , reviewBody .

The second part is to  build a sentiment classifier to classify reviews. I did this by training and testing a BoW text classifier on the provided review dataset using RatingValue as labels. The ratings are binned into negative (ratings 1 & 2 ), neutral (rating 3 ) and positive (ratings 4 & 5 ) sentiment. The binned ratings are coded with negative as 0 , neutral as 1 and positive as 2.The data is splited into training and validation sets and the validation data is used for model selection and evaluation. For this part, performance is reported in accuracy, F1-score and a confusion matrix.

This part has the same goal as part 2, that is, to classify the sentiment of reviews from Trustpilot.com. The same dataset is used. However, this time, I have to beat your previous performance (specifically, I need to get more than 60% accuracy on the test set). To do this, I will be encoding the reviews with a neural language model followed by sentiment classification. 
