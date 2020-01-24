# Article Theme Classification Based on Titles
# Proposal

## Problem Statement

Numerous articles are being posted on the internet on a daily basis. For a platform that facilitates members sharing their ideas through writing and reading, creating an index system for information of such a high volume can be a challenging task. Although there are many flavors of systems available, there are two general families, keywords and themes.

Key-word-based systems give authors the freedom to label their own work. By specifying key words or #tags, the authors allow readers to search for information that aligns with their interest through author-generated labels. Albeit very flexible and dynamic, a keyword-based index system can be very costly to implement and maintain. Because key words may be submitted by the author in a somewhat arbitrary way, it embeds uncertainty in the process of searching and retrieving information. For instance, a word may have various cases and derivations, and different words can also be semantically similar. In order for the reader’s search to hit the target accurately and comprehensively, the index system has to be able to understand different cases and variations of the same word, as well as establish semantic similarity.

On the other hand, a theme-based system only allows articles to be labeled with predefined topics. Instead of dealing with a potentially infinite number of keywords, a theme-based index system can be more structurized, and help readers quickly narrow down the scope of their search. Such advantages make it an ideal complementary system to keywords.

This project aims to explore different machine learning approaches and models that can automate the task of classifying articles into different themes according to their titles. Although the authors of the articles could provide their own themes, an automatic algorithm can suggest the most likely category to the publisher, and help promote a consistent framework that facilitates a more robust and efficient indexing and searching system.

## Data Source

The data source comes from Kaggle (Medium Post Titles — Medium Post Titles, Subtitles, Categories, https://www.kaggle.com/nulldata/medium-post-titles). It contains the titles of 126,095 articles posted on Medium (https://medium.com). These articles belong to and are labeled with about 100 different themes.

## Approach

### Exploratory analysis

The project will experiment with some natural language processing tools to transform the texts to numerical data which are ready for machine learning algorithms. Several tentative approaches will be utilized to summarize and visualize the data, such as frequency analysis and wordcloud visualization. These methods can provide an intuitive landscape, which will benefit making sensible choices regarding feature extraction and machine learning algorithms.

### Naive Bayes classification

This project will build a naive Bayes classifier as a benchmark classifier. The texts will be transformed into vector representations. A multinomial naive Bayes model can be fit to the training data while hyperparameters are being tuned via cross validation. A held-out set of data will be used to evaluate the performance of the final model

### Neural network

This project will test several different kinds of neural networks — multilayer perceptron network, fully recurrent neural network and long short-term neural network. Different choice of structures and hyperparameters will be experimented to find the relatively optimal setup.

## Expected Outcome

The project should deliver a comprehensive report that documents the performance of neural networks with different architectures in the task of theme classification of article titles. 
