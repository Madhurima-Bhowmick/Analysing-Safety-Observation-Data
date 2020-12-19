# Textinator


In this project, I have performed Text Mining on sample test data and created a sentiment detector using GUI.

#### What is Text Mining?

Text Mining is the process of deriving high quality informationfrom text. It involves the discovery by computer of new, previously unknown information, byautomatically extracting information from different written resources.

It usually involves the process of structuring the input text, deriving patterns within the structured data, and finally evaluation and interpretation of the output.

### Packages to be installed :
1. pandas
2. nltk
3. os
4. matplotlib
5. tkinter
6. numpy


### Steps involved in Text Mining :
1. Tokenization
2. Frequency Distribution
3. Stopwords
4. Stemming
5. Lemmatization
6. POS Tagging
7. Sentiment Analysis


#### 1. Tokenization


Tokenization is the process of turning a meaningful piece of data, into a random string of characters called a token that has no meaningful value if breached. Tokens serve as reference to the original data, but cannot be used to guess those values. 

Tokens are the building blocks of Natural Language. Tokenization is a way of separating a piece of text into smaller units called tokens. Here, tokens can be either words, characters, or subwords.

In this section, word_tokenize of nltk is imported and then the sample input text is passed to it. The sentence is then divided into word tokens.



#### 2. Frequency Distribution

A frequency distribution tells us the frequency of each vocabulary item in the text. In general, it could count any kind of observable event. It is a distribution because it tells us how the total number of word tokens in the text are distributed across the vocabulary items.

Here, FreqDist is imported from nltk to find the frequency distinct of the tokenized text and frequency of all words is also calculated. Using matplotlib, frequency distribution graph is plotted.



#### 3. Stopwords

Stop words are a set of commonly used words in any language. For example, in English, “the”, “is” and “and”, would easily qualify as stop words. In NLP and text mining applications, stop words are used to eliminate unimportant words, allowing applications to focus on the important words instead.In computing, stop words are words which are filtered out before or after processing of natural language data.

Here, stopwords of nltk is imported and then the stopwords are found out from english language. The tokenized text is then iterated and the stopwords are removed to get the filtered sentence.



#### 4. Stemming

Stemming is the process of reducing a word to its word stem that affixes to suffixes and prefixes or to the roots of words known as a lemma. Stemming is the process of producing morphological variants of a root/base word. Stemming programs are commonly referred to as stemming algorithms or stemmers. A stemming algorithm reduces the words, for example “chocolates”, “chocolatey”, “choco” to the root word, “chocolate” and “retrieval”, “retrieved”, “retrieves” reduce to the stem “retrieve”. 

In this section, PorterStemmer of nltk is imported and stemming is performed on the filtered sentence. 



#### 5. Lemmatization

Lemmatization usually refers to doing things properly with the use of a vocabulary and morphological analysis of words, normally aiming to remove inflectional endings only and to return the base or dictionary form of a word, which is known as the lemma. Lemmatization, on the other hand, takes into consideration the morphological analysis of the words.

Here, WordNetLemmatizer is imported from nltk and then lemmatize function is called to perform lemmatization on the filtered text.



#### 6. POS Tagging

Part-Of-Speech tagging (POS tagging or PoS tagging or POST), also called grammatical tagging is the process of marking up a word in a text (corpus) as corresponding to a particular part of speech, based on both its definition and its context. A POS tag is a special label assigned to each token (word) in a text corpus to indicate the part of speech and often also other grammatical categories such as tense, number (plural/singular), case etc. POS tags are used in corpus searches and in text analysis tools and algorithms.

pos_tag function of nltk is called and the tokenized text is passed to perform POS tagging.



#### 7. Sentiment Analysis

Sentiment analysis (opinion mining) is a text mining technique that uses machine learning and natural language processing (nlp) to automatically analyze text for the sentiment of the writer (positive, negative, neutral, and beyond). Sentiment Analysis is the process of determining whether a piece of writing is positive, negative or neutral. Sentiment analysis helps data analysts within large enterprises gauge public opinion, conduct nuanced market research, monitor brand and product reputation, and understand customer experiences.

Here, SentimentIntensityAnanlyzer is imported from vaderSentiment. polarity_scores method is called to find the sentiment of the input text, whether it is positive, negative or neutral. A GUI window is then created to calculate and display the sentiment of the text.


### GUI Window Screenshot


![Capture](https://user-images.githubusercontent.com/76059423/102685916-f35c8d80-4209-11eb-9c97-4773989dad2a.PNG)
