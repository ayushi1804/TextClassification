# TextClassification
In this project, I read text documents and classified them into 20 classes. The data used for training and testing can be found here- https://archive.ics.uci.edu/ml/machine-learning-databases/20newsgroups-mld/

# Tools AND Libraries Used
1. os
2. numpy
3. matplotlib
4. ntlk-corpus
5. nltk-tokenize

The input data contains 20000 files belonging to 20 classes hence 1000 files from each class.
The output is 2000 classes.

Firstly I read the text files using os. I converted the files into a list of words by tokenizing it and and then I removed punctuation and stopwords.Then I created a dictionary of all the words and their frequencies. I plotted this and extracted the mostly used 2000 words. These features will act like features.

Then I again read the files and created an input array of dimension 20000*2000, in which for all the 20000 files I stored the frequencies of each feature in that file. The output is a 20000*1 array.

Then I split my data into training and testing, and then I implemented naive bayes classifier.
Finally I compared my result with that of the inbuilt multinomial naive bayes classifier.
