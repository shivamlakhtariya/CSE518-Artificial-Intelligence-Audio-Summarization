# CSE518-Artificial-Intelligence-Audio-Summarization

## Audio Summarization System


## Table content

- ALgorithm
- Introduction
- Functionality
- Approach
- Results
- Contributors


## Algorithm
- Term Frequency and Inverse Document Frequency (Tf-idf) Summarizer
- Frequency based Summarizer
- Gensim based summarizer
- Gensim with LDA and Mallet's allocation
- Speech to text converser


## Introduction
Recommendation systems enable users to access products that they may not be aware of. The two traditional recommendation techniques are content-based and collaborative filtering. While both methods have their own advantages, they also have certain disadvantages, some of which can be solved by combining both techniques to improve the quality of the recommendation. Broadly speaking, a recommendation system provides specific suggestions about items (products or actions) within a given domain, which may  interest the given active user.

Product recommendation is generally a filtering system which seeks to predict, display and suggest the product to users that they would like to purchase. This type of system is utilized in a variety of fields such as news, research articles and many more.

Here we have designed a product recommendation system which can provide appropriate suggestions to the customers while buying another products. We are designing the system such that it suggests the item based on the ratings of all the other items and also according to their purchase history.It helps the users to make a right choice and also it makes the content more personalised.


## Functionality

- We are recommending the products based on the ratings of the products given by the other customers or users in past using cosine similarity as well as jaccard similarity.
- When a new user comes to buy a product and enters a keyword to search, we are recommending the products using k-mean text clustering based on the keyword .
- We are performing clustering based on the product ID and ratings given to that particular product.
- We have performed k-means clustering from scratch without the use of inbuilt functions.


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

# GSM based algorithm's efficiency w.r.t. time for book "Honest Abe"
<img src="https://github.com/shivamlakhtariya/CSE518-Artificial-Intelligence-Audio-Summarization/blob/main/Results/GSM%20Efficiency.JPG" width="800" height="500">

# Choosing a number of topic for LDA algorithm w.r.t. coherence score
<img src="https://github.com/shivamlakhtariya/CSE518-Artificial-Intelligence-Audio-Summarization/blob/main/Results/Choosing-the-optimal-number-of-LDA.png" width="800" height="500">

# Frequency based summarizer output for total length = 0.2 of total speech and vodeo is "https://www.youtube.com/watch?v=jtpOYxsZj7o"
<img src="https://github.com/shivamlakhtariya/CSE518-Artificial-Intelligence-Audio-Summarization/blob/main/Results/frequency%20based%20summarizer%20output.JPG" width="650" height="400">

# Gensim based summarizer output for total length = 0.3 of total speech and vodeo is "https://www.youtube.com/watch?v=jtpOYxsZj7o"
<img src="https://github.com/shivamlakhtariya/CSE518-Artificial-Intelligence-Audio-Summarization/blob/main/Results/Gensim%20based%20algorithm%20output.JPG" width="900" height="550">


# pyLDAvis
<img src="https://github.com/shivamlakhtariya/CSE518-Artificial-Intelligence-Audio-Summarization/blob/main/Results/pyLDAvis.png" width="900" height="550">


## Contributors

| [Dhruvanshu Parmar](https://github.com/Nisargpatel16)                                                                                                            
| [Shivam Lakhtariya](https://github.com/shivamlakhtariya)     
| [Aditya Raj](https://github.com/raj49274)

