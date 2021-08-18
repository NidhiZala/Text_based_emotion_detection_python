Name:- Nidhi Zala

Student ID:- 1160480

Email ID:- nzala@lakeheadu.ca


# Text Based Emotion Detection using Python


## Table of Contents

1. Introduction
2. Dataset
3. Methodology
5. Results and Discussion
6. Conclusion
7. References

## Introduction
With the advent of new technologies, a connection between emotions and other fields have evolved and become evident. Considering major streams like marketing, human interface and especially social media, emotions play a vital role in holding up their users. In today’s world of social media, when with each move by the user, such a large amount of data is generated emotions are one of the vital considerations taken into account for further analysis. With this project, I propose a model to detect emotions of the text which can further be utilized in multifarious fields for analysis of emotions leading to more user interaction. Analysing the literature review for the topic many unsupervised and supervised approaches have been used by developers till date. This project  tries multiple techniques and find the most efficient method for detecting emotions in a given text.

## Dataset 

The dataset used in the project is [text_emotion.csv](https://data.world/crowdflower/sentiment-analysis-in-text) which contains around 40000 tweets for which the emotion detection is performed.Below shows a snippet of the dataset which is cleaned after preprocessing it.
![data2](https://user-images.githubusercontent.com/38599806/129970155-ca0d21c7-870a-4578-bdb8-9817f3b5e919.JPG)


## Methodology

The project follows the following steps as shown in the below flowchart:

![image](https://user-images.githubusercontent.com/38599806/129970277-18549ee6-19ef-45aa-917d-eed4b431e3ff.png)

Initially the method startes with selecting and loading the dataset. Later after taking an overview of the dataset cleaning is performed by removing unwanted columns and later with preprocessing, html tags, punctuations and all are removed to acquire the final data to be used further. After proprocessing Feature Selection is done by using TFIDF vectorizer and Count vectorizer. To examinf which feature selection technique works the best both for tfidf and count vectors models are trained seperatly. The following 4 models are used :

1. Naive bayes classifier
2. Random forest Classifier
3. Linear Support Vector Machine 
4. Logistic Regression

After training the data for both feature techniques the outcomes for 4 models are examing and results are decided.

## Results and discussion

The below image displays common accuracies for algorithms and feature techniques :
![image](https://user-images.githubusercontent.com/38599806/129971380-66e5fc9a-ea49-4b59-a751-b2c977b6de2c.png)

Thus it is visible that Linear SVM with count vectorizer performs the best in terms of accuracy and Tfidf vectorizer shows the lest accuracies for all the models compared to Count Vectorizer.

## How to run this project:

1. In Github the uploaded file can be ran in Google Colab. 
2. Click on the google colab icon and try to run the project.
3. For nltk error, download stopwords and wordnet as these are not available by default in google colab.

## Conclusion

The project efficiently compares various machine learning models for emotion detection and finds the one that performs the best. Also it compares feature selection techniques and detects emotions from textual twitter data taken efficiently.

## References 

1. https://medium.com/the-research-nest/applied-machine-learning-part-3-3fd405842a18
2. https://data.world/crowdflower/sentiment-analysis-in-text

