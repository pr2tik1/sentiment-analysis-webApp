# SageMaker Deployment Project

The notebook and Python files result in a simple web app which interacts with a deployed recurrent neural network performing sentiment analysis on movie reviews. This project was part of my Udacity's nanodegree course. The goal is to understand the scalable machine learning tasks using AWS sagemaker. The model uses LSTM network.

## Getting Started

For the web app to work we require AWS SageMaker, AWS S3 Bucket, AWS Lambda, AWS API Gateway. Within AWS Sagemaker the ml.t2.medium instance to run the notebook. Inside the notebook ml.p2.xlarge is used for training a model and ml.m4.xlarge is used for deployment.  

## Dataset
We will be using the IMDb dataset, which contains 25,000 highly polar movie reviews for training, and 25,000 for testing. An example of a postive review is given below

```
The violent and rebel twenty-five years old sailor Antwone Fisher (Derek Luke) is sent to three sessions for evaluation with the navy psychiatrist Dr. Jerome Davenport (Denzel Washington), after another outburst and aggression against a superior ranked navy man. Reluctant in the beginning of the treatment, he gets confidence in Dr. Davenport and discloses his childhood, revealing painful traumas generated in his foster house. Meanwhile, he meets Cheryl Smolley (Joy Briant), and they fall in love for each other. Resolving his personal problems, Antwone becomes a new man. This true familial drama is a touching and positive story of a man who finds a friend and is sent back to a regular life. The direction of Denzel Washington is excellent, making sensitive, attractive and with good taste, a story about child abuse. In the hands of another director, it might be a very heavy story. My vote is eight.

Title (Brazil): 'Voltando a Viver' ('Returning to Live')
```


### Requirements

The libraries required to install for sentimental anlaysis and deployment of web app. 

```
torch 
pandas
numpy
nltk
beautifulsoup4
html5lib
```

### Installing

1. Initialize AWS instance and the jupyter notebook then run SageMaker Project.ipynb
  
```
ipython SageMaker-Project.ipynb
```

2. Then create Lambda function and API Gateway for the web app, as shown in notebook.

3. Edit the html with API link from AWS API Gateway

4. Run the html file

5. Type the sentiment and click submit

## Glimpse of the Web Application

![alt text](https://github.com/pr2tik1/sentiment-analysis-webApp/blob/master/sentimental-webapp.jpg?raw=true)

## Built With

* [PyTorch](https://pytorch.org/) - Deep Learning Framework
* [AWS Sagemaker](https://sagemaker.readthedocs.io/en/stable/) - Cloud Services for Machine Learning

## Acknowledgments

* Credits to udacity community and instructors.

