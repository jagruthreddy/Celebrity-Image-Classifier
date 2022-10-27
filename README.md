# Celebrity-Image-Classifier
Celebrity recognition using machine learning

## Table of Content
  * [Overview](#overview)
  * [Local Setup](#local-setup)
  * [Steps](#steps)

## Overview
Our main goal is to build a website in which you can drag and drop an image of sports person and it will tell you which sports person that is.<br />
We are restricting our image classification to only five classes<br/>
**Steps:** <br/>
1) TEXT PREPROCESSING
2) VECTORIZATION
3) TERM FREQUENCY-INVERSE DOCUMENT FREQUENCY(TF-IDF)
4) CLASIFICATION ALGORITHMS <br/>

**Screenshot:**
<br />
[![](https://imgur.com/a/XDR2phY/Dynlly3.png)](https://imgur.com/a/XDR2phY)<br />

## Local Setup
Clone the repository on your local environment <br>

```bash
git clone https://github.com/jagruthreddy/news-classification
```
Navigate to the folder <br>
```bash 
cd news-classification
```
USE GOOGLE COLAB OR JUPYTER NOTEBOOK<br>


## Steps
### 1) TEXT PREPROCESSING:
**TOKENIZATION:** This process divides a large piece of continuous text into distinct units or tokens basically this process is often known as tokenization.<br />
**STEMMING:** This is the idea of removing the suffix of a word and reducing different forms of a word to a core root.<br />
**STOPWORDS REMOVAL:** A stop word is a commonly used word (such as “the”, “a”, “an”, “in”) that a search engine has been programmed to ignore.<br />

### 2) VECTORIZATION:
**Scikit-learn** library offers easy-to-usetools to perform feature extraction of your text data that is Vectorization.The vectorization is a technique used to convert textual data to numerical format. Using vectorization, a matrix is created where each column represents a feature and each row represents an individual review.
### 3) Term Frequency-Inverse Document Frequency(TF-IDF)
**TD-IDF** basically tells importance of the word in the corpus or dataset <br />
• It is the combination of Term frequency and Inverse Document Frequency. <br />
• Inverse Document frequency is another concept which is used for finding out importance of the word. It is based on the fact that less frequent words are more informative and important.<br />
**IDF(t)** = log_e(Total number of documents / Number of documents with term t in it) <br />
**WI,J**=weight which signifies how important a word is for individual text message. <br />
![](https://i.imgur.com/uJMS59V.png)
### 4) CLASIFICATION ALGORITHMS
**Logistic Regression** <br />
Logistic Regression is a Machine Learning algorithm which is used for the classification problems. Logistic function: 1 / (1 + exp(-x)) normalizes everything to be between 0 and 1. 
## Technologies Used
![](https://forthebadge.com/images/badges/made-with-python.svg)

[<img target="_blank" src="https://upload.wikimedia.org/wikipedia/commons/thumb/2/2d/Tensorflow_logo.svg/1915px-Tensorflow_logo.svg.png" width=170>](https://www.tensorflow.org/) [<img target="_blank" src="https://seeklogo.com/images/M/matplotlib-logo-7676870AC0-seeklogo.com.png" width=280>](https://matplotlib.org/) [<img target="_blank" src="https://scikit-learn.org/stable/_static/scikit-learn-logo-small.png" width=200>](https://scikit-learn.org/stable/) 
