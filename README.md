# Text-Analytics-on-Amazon-Cell-Reviews-and-Ratings

The project analysis investigates the reviews on mobile phones that are sold
on Amazon.com with an objective of finding product and consumer insights based on price,
ratings and reviews. We also try to analyze the trends based on the relationship between
the three.

This dataset contains 82,815 reviews from Amazon about cell phones from 2004 until Sep 2019.
Each review can be associated with an item and brand name and comes with a rating ranging from
1 to 5. This makes the dataset a perfect sample for text analytics and sentiment classification.

Observing trends using price, ratings and reviews of each brand. Text data cleaning includes crteating
a dataframe to put reviews and ratings together, converting text columns into lowercase, removing stopwords,
numeric values in reviews, special characters and then word tokeninzing.
- More than 50% of reviews are recorded under Samsung and then followed by Motorola and Apple.
- Xiamoi tops the list of average rating per each brand.
- We can observe ratings in 2015 and 2014 are high when compared to recent years.
- Products whose price ranging from $50-$300 has highest number of reviews and most of the
ratings range from 2.5 to 3.5.

Applying Count vectorizer and Tf-iDF vectorizer techniques to give the metric value to every
word in each document present in the column title _y. To classify each word in the text to a topic
we are using LDA and NMF topic modelling techniques after performing vectorization techniques. 
Using PyLDAVis module to plot the topics created to know overall term frequency and estimated term frequency 
for each term in each topic.

Coming to the classification part it is more of a trial and error approach applying different calssification algorithms 
like Logsitic regression, SVM, Random Forest and Decision Trees where all the algorithms result in predicting accuracy round 70%.

Also tried predicting using a simple Conv1D network which resulted in 85% of accuracy.






