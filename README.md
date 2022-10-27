# Celebrity-Image-Classifier
Celebrity recognition using machine learning

## Table of Content
  * [Overview](#overview)
  * [Local Setup](#local-setup)
  * [Steps](#steps)
  * [Additional info](#additional-info)

## Overview
Our main goal is to build a website in which you can drag and drop an image of sports person and it will tell you which sports person that is.<br />
We are restricting our image classification to only five classes<br/>

**Project ouline:** <br/>
[![DpuIVa.md.png](https://iili.io/DpuIVa.md.png)](https://freeimage.host/i/DpuIVa)<br />
**Steps:** <br/>
1) Data collection
2) Data cleaning
3) Model
4) Classification algorithm <br/>

**Screenshot:**<br />
[![DpnQxj.md.jpg](https://iili.io/DpnQxj.md.jpg)](https://freeimage.host/i/DpnQxj)

## Local Setup
Clone the repository on your local environment <br>

```bash
git clone https://github.com/jagruthreddy/Celebrity-Image-Classifier
```
Navigate to the folder <br>
```bash 
cd Celebrity-Image-Classifier
```
GOOGLE COLAB OR JUPYTER NOTEBOOK CAN BE ONLY USED TO READ THE IPYNB File.<br>
USE PYCHARM.

## Steps
### 1) Data collection:
Data collection is the process of gathering. You can do Web scrapping or use Chrome extension or buy from 3rd party vendors<br />
### 2) Data cleaning:
Data cleaning is the process of fixing or removing incorrect, incorrectly formatted, duplicate data.<br>
1) We can remove images of multiple celebrities who are not in our class. For example, if there is a photo of Dhoni and Virat, we can remove it because Dhoni is not in our class.<br> 
We can remove images where is one eye or where face is not clear.

[![DpGAfS.md.png](https://iili.io/DpGAfS.md.png)](https://freeimage.host/i/DpGAfS)

[![DpMAhv.md.png](https://iili.io/DpMAhv.md.png)](https://freeimage.host/i/DpMAhv)

2) After Some Manual cleaning we take raw images and do Grayscaling of an images using openCV. Advantages are Dimension reduction(grayscale images are single dimensional), Reduces model complexity, For other algorithms to work(Many algorithms are customized to work only on grayscale images e.g. Canny edge detection).<br>

3) Crop faces with 2 eyes using haar cascade(It is an Object Detection Algorithm used to identify faces in an image or a real time video. The algorithm uses edge or line detection features), if two eyes are detected then only we save that image otherwise discard it. <br>

4) We use these cropped images and convert them into wavelet transformed images. In a wavelet transformed image ,you can see edges clearly and that can give us clues on various facial features such as eyes,nose,lips etc.
[![DpWrrB.md.png](https://iili.io/DpWrrB.md.png)](https://freeimage.host/i/DpWrrB)
### 3) Model:
1) Images in cropped folder are used for model training. We will use these raw images along with wavelet transformed images to train our classifier.
2) Now we use GridSearch to try out different models with different paramets.
3) Goal is to come up with best model with best fine tuned parameters

## Additional info
[Article for haar cascade](https://docs.opencv.org/3.4/db/d28/tutorial_cascade_classifier.html) <br>
The .idea directory contains a set of configuration files (. xml) for your project(PyCharm).<br>

1. Use anaconda interpreter(python 3.6) in pycharm
2. use scikit-learn 0.20.0 version in pycharm.
3. Install other libaries which are required.
<br>

Thanks to [rnikhori](https://github.com/rnikhori/) 

## Technologies Used
![](https://forthebadge.com/images/badges/made-with-python.svg)

[<img target="_blank" src="https://seeklogo.com/images/M/matplotlib-logo-7676870AC0-seeklogo.com.png" width=280>](https://matplotlib.org/) 
[<img target="_blank" src="https://scikit-learn.org/stable/_static/scikit-learn-logo-small.png" width=200>](https://scikit-learn.org/stable/) 
