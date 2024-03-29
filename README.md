# hack-a-thing-1-mikezhu

## Sept 21, 2019

## Description

For my hackathing, I followed a sentiment analysis tutorial for Python/scikit-learn and implemented the script into a website built on Meteor, a platform for creating web apps in JS. I wanted to work with something that involved machine learning, which I am interested in, and sentiment analysis seemed like a good choice. Also, I had never created a website before (I haven't taken CS52) so I wanted to learn the basics for that using an up and rising platform.

The website is super simple, as I just wanted to learn the basics for creating a website, so it essentially just takes a phrase and uses the back-end mdoels to predict the sentiment of that phrase.

The tutorials for creating the sentiment analyzer and a basic React website built on Meteor are found at
- https://stackabuse.com/python-for-nlp-sentiment-analysis-with-scikit-learn/
- https://www.datacamp.com/community/tutorials/k-nearest-neighbor-classification-scikit-learn
- https://stackabuse.com/implementing-svm-and-kernel-svm-with-pythons-scikit-learn/
- https://www.meteor.com/tutorials/react/creating-an-app
- https://docs.meteor.com/api/methods.html#Meteor-call
- https://reactjs.org/docs/forms.html
- https://github.com/extrabacon/python-shell

## Work

I worked by myself on this assignment!

## What did and didn't work

The sentiment analysis tutorial was very thorough, so I essentially used the code they provided to create the sentiment analysis tool. This was also great review for the material I learned in CS74 (Machine Learning), which I took last year.

The sentiment analysis tutorial also chose to use the RandomForestClassifier; I wanted to try different machine learning algorithms to see if there were any that provided a better accuracy, so I also tried the K-nearest neighbors (KNN) algorithm and the support vector machine (SVM) models. Both tutorials were provided above. The SVM model provided the highest accuracy on the same test set, so I decided to utilize the SVM classifier in my sentiment analysis tool.

It was initially challenging to download all the dependencies for Meteor and then Meteor itself, but once I had finished installing everything, the Meteor/React tutorial was super helpful and very easy to use.

Ultimately, I found a great way to connect the Python script to the Meteor backend server, but could not do it in a way that allowed the Python script to finish running before returning a result. In other words, my "result" on the front-end was always undefined, as the Python script would take a while to run. I tried various solutions (e.g. await/async, Future, Promises) for a long time, but just couldn't figure out a solution for that. As a result, this project isn't functionally complete, as I couldn't figure out how to connect the two separate parts. 

I also couldn't figure out how to take in user input and put that input into the classifier for it to create a prediction. This is something that I do hope to figure out just for my own sake.

Altogether, despite its shortcomings, this project was still a great way to learn a little bit about basic web dev and the challenges within web dev, and also to review machine learning and the various algorithms that are made easy to use through scikit-learn and Python.


