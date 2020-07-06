# Sentiment-Analysis-On-restaurants
Ability to clean yelp and facebook data and retrieve the aspects along with its polarity to identify the sentiments of customers towards the restaurant.

It is understood that the research area of sentiment analysis, opinion mining, sentiment mining and sentiment extraction has gained popularity.
Sentiments or opinions from social media provide the most up-to-date information, due to the proliferation of social media and the low barrier for posting the message. User generated reviews, like those found on Yelp, have become important reference material in decision making, like dining, shopping and entertainment.
With the sentiment analysis approach of business reviews, the solution is to provide customers perception using a large dataset of reviews from customers
in Yelp. Several essential aspects are addressed within the scope of this survey where thevrestaurants can have some vital inputs to improve in their aspects which may directly influence their business. In this research, we propose following approaches for sentiment analysis: N-Grams and Aspect Extraction using Spacy to determine the frequency of each aspect and detect the polarity. We have then focused on comparing the polarity of the aspects amongst the three given restaurants. The analysis led to some interesting conclusions which could help any business to flourish by enhancing customer satisfaction and meeting their expectations.


# Methodology
To evaluate the performance of the restaurant, it is key to identify the negatives and positives of each aspect of the restaurant. Sentiment analysis is based on textual data analysis that signifies the customers opinions towards the product or service. We will therefore retrieve the opinions of the restaurant’s aspects, which are either positive, negative or neutral. From the acquired user generated dataset from Yelp, the sentiments of the restaurant’s aspects are identified through a series of steps that involves Data Profiling, Data Pre-processing, Aspect Extraction and Aspect Polarity. 


# Data Pre-processing
Pre-processing the data is the process of cleaning and preparing the text for further analysis. Data cleaning, in this scenario, textual data cleaning usually consists of a series of steps to attain data in a clean format. They are aligning any case mismatch, removing special characters, filling missing or blank data, removal of noise, etc. Therefore, it is the dataset and the analysis required that defines the process of data cleaning. In this scenario, online texts usually contain lots of noise and uninformative parts such as HTML tags, scripts and advertisements. In addition, on a word level, many words in the text do not have an impact on the general orientation of the sentence. Keeping those words puts the dimensionality of the problem high and hence the sentiment analysis would be more difficult since each word in the text is treated as one dimension. 

1. Lowercasing
The first pre-processing step which we will do is transform our review texts into lower case. This avoids having multiple copies of the same words. For example, while calculating the word count, ‘Analytics’ and ‘analytics’ will be taken as different words.

2 Removing Punctuation
The next step is to remove punctuation, as it does not add any extra information while treating text data. Therefore, removing all instances of it will help us reduce the size of the training data.

3 Removal of Stop words
As we discussed earlier, stop words (or commonly occurring words) should be removed from the text data. For this purpose, we can either create a list of stopwords ourselves or we can use predefined libraries. 

4. Stemming vs lemmatization
Stemming refers to the removal of suffices, like “ing”, “ly”, “s”, etc. by a simple rule-based approach. For this purpose, we will use PorterStemmer from the NLTK library. Lemmatization is a more effective option than stemming because it converts the word into its root word, rather than just stripping the suffices. It makes use of the vocabulary and does a morphological analysis to obtain the root word. Therefore, we usually prefer using lemmatization over stemming. 

# Sentiment Analysis Using Textblob
Sentiment analysis is basically the process of determining the attitude or the emotion of the writer, i.e., whether it is positive or negative or neutral. The sentiment function of textblob returns two properties: polarity, and subjectivity. Polarity is a float which lies in the range of [-1,1] where 1 means positive statement and -1 means a negative statement. Subjective sentences generally refer to opinion, emotion or judgment whereas objective refers to information. Subjectivity is also a float which lies in the range of [0,1].

Above analysis can be referred in the respective python notebook file from the repository and acknowledge the workings.
   
