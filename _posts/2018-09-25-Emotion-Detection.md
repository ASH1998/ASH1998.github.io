---
layout: post
title:  "Emotion Detection"
date:   2018-09-25
desc: "Emotion Detection using bi-CNN"
keywords: "Ashutosh,Python,CNN,Image-Processsing,blog,easy"
categories: [Deep Learning]
tags: [Emotion, CNN, Python, Deep-Learning]
icon: icon-html
---

# Emotion-detection
[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/dwyl/esta/issues)  [![HitCount](http://hits.dwyl.io/ASH1998/Emotion-detection.svg)](http://hits.dwyl.io/ASH1998/Emotion-detection)

Emotion Detection using deep unbaised CONV-net!!
## Website : [https://ash1998.github.io/Emotion-detection/](https://ash1998.github.io/Emotion-detection/)

## Getting Data
The dataset used here is the famous `FER2013 dataset` from kaggle's [FER challenge of 2013](https://www.kaggle.com/c/challenges-in-representation-learning-facial-expression-recognition-challenge) 
### Download 
##### Zip File : [from here 92MB](https://www.kaggle.com/c/3364/download-all)    

##### Using API :     
1.Install Kaggle from [github](https://github.com/Kaggle/kaggle-api)   
2.Use the command in terminal `kaggle competitions download -c challenges-in-representation-learning-facial-expression-recognition-challenge`    

Docs on Kaggle API usage :
[github](https://github.com/Kaggle/kaggle-api) | [kaggle](https://www.kaggle.com/docs/api)

## Dependencies
1. Python
2. Jupyter
3. Keras
4. Tensorflow
5. Matplotlib
6. Pandas
7. Numpy
8. tqdm
   

## Usage
### For model1:      
1. Download the data and unzip it as `FER2013` dir.
2. Clone this repo.
3. Add the full path of `fer2013.csv` into `cell 3` of `FER2013-model1.ipynb`.
4. Run the file or use the pretrained model weights.
### Using pre-trained weights:
The Layers for the network : 

![name4](https://github.com/ASH1998/Emotion-detection/blob/master/Images/4.PNG)

### For EDA notebook :     
1. Change the path to weights folder in `cell3`.      
## Images
Testset Accuracy : 

![image2](https://github.com/ASH1998/Emotion-detection/blob/master/Images/2.PNG)

Some Images prediction :

![image5](https://github.com/ASH1998/Emotion-detection/blob/master/Images/5.PNG)   
![image1](https://github.com/ASH1998/Emotion-detection/blob/master/Images/1.PNG)       
![image3](https://github.com/ASH1998/Emotion-detection/blob/master/Images/3.PNG)           
![image6](https://github.com/ASH1998/Emotion-detection/blob/master/Images/6.PNG)   
![image7](https://github.com/ASH1998/Emotion-detection/blob/master/Images/7.PNG)   

## EDA confusion Matrix and Scores:
![image8](https://github.com/ASH1998/Emotion-detection/blob/master/Images/811.PNG)      
![image9](https://github.com/ASH1998/Emotion-detection/blob/master/Images/9.PNG)         
![image10](https://github.com/ASH1998/Emotion-detection/blob/master/Images/10.PNG)   

### ED Analysis:
1. `Happy` Emotion is the most detected, as it has most number of examples
2. `Sad`, `Surprise`, `Neutral` and `Anger` are also good in detecting due to enough examples.
3. `Fear` and `Disgust` perform worse, possible reasons : Less training examples and for `disgust`: pretty similar to `anger` features.
4. `Sad` emotions are also closely detected as `neutral`, cuz its hard to distinguish them with just this much data.
