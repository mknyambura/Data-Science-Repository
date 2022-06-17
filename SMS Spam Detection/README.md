# SMS-Spam-Detection

### I will be using the multinomial Naive Bayes implementation.

#### This particular classifier is suitable for classification with discrete features (such as in our case, word counts for text classification). It takes in integer word counts as its input. 

#### On the other hand Gaussian Naive Bayes is better suited for continuous data as it assumes that the input data has a Gaussian(normal) distribution.

## Bag of Words Approach

#### Most Machine Learning algorithms rely on numerical data to be fed into them as input, and email/sms messages are usually text heavy.

### We need a way to represent text data for machine learning algorithm and the bag-of-words model helps us to achieve that task. It is a way of extracting features from the text for use in machine learning algorithms.

### In this approach, we use the tokenized words for each observation and find out the frequency of each token.

### Using a process which we will go through now, we can convert a collection of documents to a matrix, with each document being a row and each word(token) being the column, and the corresponding (row,column) values being the frequency of occurrence of each word or token in that document.

### Lets break this down and see how we can do this conversion using a small set of documents. To handle this, we will be using sklearns count vectorizer method which does the following:
###               1. It tokenizes the string(separates the string into individual words) and gives an integer ID to each token.
###               2. It counts the occurrence of each of those tokens.
