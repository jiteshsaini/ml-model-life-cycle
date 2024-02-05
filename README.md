
# Project Overview
The project covers the complete cycle of creating, deploying and interacting with a Machine Learning model. It involves training a Logistics Regression model for a binary classification task and deploying the trained model in a webserver to obtain real-time predictions via rest API using a simple web page (created for this project).
<img src='https://github.com/jiteshsaini/files/blob/main/img/ml-model-lifecycle.png'>

## The dataset
The <a href='https://archive.ics.uci.edu/dataset/468/online+shoppers+purchasing+intention+dataset'>dataset</a> is sourced from UC Irvine repository. The dataset is designed to predict the purchase intention of an online user based on the browsing information of over 12000 online  sessions on an e-commerce website. The features of this dataset have a mix of continuous and categorical variables. Our aim is to predict the target variable 'Revenue' to determine the purchase intention of a online shopper in real-time.

## Model Deployment and Real-time predictions
The webpage is created using HTML and Javascript and designed to simulate a user’s browsing behaviour and pass the browsing parameters to the server via background ajax calls. This raw data received by the server is encoded and scaled using the pickle files, created during the training phase. This ensures that the incoming data (unseen data) is transformed in a format that is similar to the data format used while training the model. The processed data is fed to the model for inference and predictions are obtained. The predictions are transmitted back to the browser and displayed on the web page.

<img src='https://github.com/jiteshsaini/files/blob/main/img/model-deployment.gif'>
