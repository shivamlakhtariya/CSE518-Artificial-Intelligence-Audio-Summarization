# CSE518-Artificial-Intelligence-Audio-Summarization

## Audio Summarization System


## Table content

- ALgorithm
- Introduction
- Approach
- Results
- Guidelines 
- Contributors


## Algorithm
- Term Frequency and Inverse Document Frequency (Tf-idf) Summarizer
- Frequency based Summarizer
- Gensim based summarizer
- Gensim with LDA and Mallet's allocation
- Speech to text converser


## Introduction
One of the primary applications of natural language processing is to automatically extract what topics people are discussing from large volumes of text. Some examples of large text could be feeds from Books, Youtube videos, movies, etc, user feedbacks, news stories, e-mails of customer complaints etc

Knowing what people are talking about and understanding their problems and opinions is highly valuable to businesses, administrators, political campaigns. And it’s really hard to manually read through such large volumes and compile the topics


## Approach

- LDA’s approach to topic modeling is it considers each document as a collection of topics in a certain proportion. And each topic as a collection of keywords, again, in a certain proportion.
- Once we provide the algorithm with the number of topics, all it does it to rearrange the topics distribution within the documents and keywords distribution within the topics to obtain a good composition of topic-keywords distribution.
- A topic is nothing but a collection of dominant keywords that are typical representatives. 


Importing data : 20 newsgroups dataset.
Preprocessing : remove stop words, punctuation mark.
Breaking down each sentence into a list of words through tokenization.
Creating Bigram and Trigram Models : Bigrams are two words frequently occurring together in the document. Trigrams are 3 words frequently occurring. Some examples in our example are: ‘front_bumper’, ‘oil_leak’, ‘maryland_college_park’ etc. Gensim’s Phrases model can build and implement the bigrams, trigrams, quad grams and more. (Threshold = 100 times)
Make that word Lemmatize (Walking -> Walk)(using Spacy library)
Create the Dictionary and Corpus for Topic Modeling : Gensim creates a unique id for each word in the document. The produced corpus is a mapping of (word_id, word_frequency). For example, (0, 1) above implies, word id 0 occurs once in the first document. This is used as the input by the LDA model.

alpha and eta are hyperparameters that affect sparsity of the topics. According to the Gensim docs, both defaults to 1.0/num_topics prior. 
The LDA model is built with 20 different topics where each topic is a combination of keywords and each keyword contributes a certain weightage to the topic. If we print the output :
Topic 0 is a represented as _0.016“car” + 0.014“power” + 0.010“light” + 0.009“drive” + 0.007“mount” + 0.007“controller” + 0.007“cool” + 0.007“engine” + 0.007“back” + ‘0.006“turn”. 
It means the top 10 keywords that contribute to this topic are: ‘car’, ‘power’, ‘light’.. and so on and the weight of ‘car’ on topic 0 is 0.016
The weights reflect how important a keyword is to that topic.
Model perplexity and topic coherence provide a convenient measure to judge how good a given topic model is.
To examine the produced topics and the associated keywords. pyLDAvis the most useful tool and it creates interactive chart.




## Libraries
- Youtube-dl
- webvtt-py
- scikit learn
- tkinter
- numpy
- TfidfVectorizer and CountVectorizer
- Pandas
- Gensim 
- pyLDAvis
- matpllotlib

## Results

# GSM based algorithm's efficiency w.r.t. time for the book "Honest Abe"
<img src="https://github.com/shivamlakhtariya/CSE518-Artificial-Intelligence-Audio-Summarization/blob/main/Results/GSM%20Efficiency.JPG" width="800" height="500">

# Choosing a number of topic for LDA algorithm w.r.t. coherence score
<img src="https://github.com/shivamlakhtariya/CSE518-Artificial-Intelligence-Audio-Summarization/blob/main/Results/Choosing-the-optimal-number-of-LDA.png" width="800" height="500">

# Frequency based summarizer output for total length = 0.2 of total speech and vodeo is "https://www.youtube.com/watch?v=jtpOYxsZj7o"
<img src="https://github.com/shivamlakhtariya/CSE518-Artificial-Intelligence-Audio-Summarization/blob/main/Results/frequency%20based%20summarizer%20output.JPG" width="650" height="400">

# Gensim based summarizer output for total length = 0.3 of total speech and vodeo is "https://www.youtube.com/watch?v=jtpOYxsZj7o"
<img src="https://github.com/shivamlakhtariya/CSE518-Artificial-Intelligence-Audio-Summarization/blob/main/Results/Gensim%20based%20algorithm%20output.JPG" width="900" height="550">

# LDA formula
<img src="https://github.com/shivamlakhtariya/CSE518-Artificial-Intelligence-Audio-Summarization/blob/main/Results/LDA%20formula.JPG" width="700" height="500">

# pyLDAvis
<img src="https://github.com/shivamlakhtariya/CSE518-Artificial-Intelligence-Audio-Summarization/blob/main/Results/pyLDAvis.png" width="900" height="550">

# pyLDAvis for topic 1
<img src="https://github.com/shivamlakhtariya/CSE518-Artificial-Intelligence-Audio-Summarization/blob/main/Results/pyLDAvis%20Output.JPG" width="900" height="550">

# Defination of Relevance
<img src="https://github.com/shivamlakhtariya/CSE518-Artificial-Intelligence-Audio-Summarization/blob/main/Results/Relevance.JPG" width="900" height="550">


## Contributors

| [Dhruvanshu Parmar](https://github.com/DhruvanshuParmar)                                                                                                            
| [Shivam Lakhtariya](https://github.com/shivamlakhtariya)     
| [Aditya Raj](https://github.com/raj49274)

