# How to solve data problems

Solving a problem without guidance is a nightmare for a junior data scientist! Working in start-up environments as a data scientist without a senior's help can be painful. Unclear goals, high expectations, and bad management led to frustration and poor results. Fortunately, not everyone has to face the same problems I have. This document's purpose is to be a guideline for data scientists. I will teach some insights and pain points I have learned so far! Hope this will be helpful.

# 1) Understand your problem

It's not uncommon for data scientists to jump straight into data and modeling. Managers might ask for machine learning models even without knowing what they are. When these times arrive, you must take a step back and ask yourself: what am I trying to solve here? 
Sometimes the solution is very straightforward: like trying to predict a default credit customer. Other times, you need to break your problem into smaller ones: for face recognition, you first need to identify a face and then match it with your database of faces. 
However, the problem usually won't be as well defined most of the time. You will have data scattered around, and it's hard to figure things out. *You* need to create a solution that generates the most value for the company. Sure, it can be a machine learning model (or several ones), but it might as well be a dashboard, a decision-making framework using your model. It all depends on your problem needs and your creativity!

# 2) Know your data

Data can come in many formats and flavors. It can be on SQL databases or a bunch of images. It's essential to dive deep into it. Often you will face some data issues, or your dataset might not be enough to answer your questions. Fortunately, there are techniques that you can use, such as data cleansing and data augmentation, that can help you. This section will be divided depending on the format of the data.

 - Tables - most of your data will be in tables. Sometimes in a single .csv file, sometimes in a database. You will have to figure out how to access them and join these tables together. Standard practice here is to conduct an extensive *Exploratory Data Analysis*: to see what variables are numerical, text, and what needs to be categorized. Analyze them and check for frequent values using histograms and boxplots. Here are some Python libraries for this: `pandas,` `seaborn', `TensorFlow data validation.`
	
(TensorFlow data validation img)
Images -  computer vision is a growing topic in the data science field. It's becoming more often that your data will be photos and pictures. You will need to answer other problems: are the images of the same shape (width x height)? Is the resolution always the same? Are the pictures clear, or is it too bright or dark? Can a human understand it? Do I have enough examples? Your model input needs to be consistent across all the samples! You will have to crop, resize and brighten your data. You can use `PIL' library to do so in scale.
 (img data augmentation)
Mixed - sometimes, your data will be mixed, having tables, images, text, and even audio. You can then apply different techniques to each part of your data. 

# 3) Have a baseline

When your data is ready, it's finally time to start modeling. However, it is crucial to have a benchmark before the modeling phase. You can compare your ongoing results and experiments with a point of reference. Ultimately, you will have an expectation of your final product result! 
This baseline can come in many forms:
The previous model version -  your problem might be to increase an old model's accuracy or change its architecture. The old model can be used as a reliable benchmark.
Human-Level Performance - if you have professionals or specialists in the area, use them! For example, let's say the average doctor has an error rate of 3% for an image lung cancer diagnostic; use this as your baseline. Machines can be better at some tasks, but Human-Level Performance is a great reference overall.
Quick implementation - if you can't find a good benchmark, use your own! Create a simple and fast model with a few lines of code, and use it as your reference. It can be a simple linear regression without a lot of feature engineering.


# 4) Modeling time

Finally, you get to the fun part! Here is where most of us like to be: showing off our excellent data science skills through the state-of-the-art Ai models. 
Feature Engineering: After thoroughly analyzing your data and understanding the business, create new features with your insights. Linear models don't fully capture feature interactions, and you might need to create your own variables for them to have good results. 
Machine Learning Models - You can try different techniques and libraries depending on your problem. You might try logistic regression, gradient boosting trees, random forests, and even neural networks for classification tasks. For images, you can use convolutional neural networks with different architectures.
Ensemble - when you achieve good models, you can always ensemble your solution and have a better model. Combining different models can lead to an incredible accuracy increase. This is standard practice in many Kaggle competitions but might be too complex or challenging in real problems. Use it at your own risk.


# 5) Validate your model

The only way to know your model accuracy honestly is to measure it in unseen data. That's why it is vital to split your data into training and testing datasets:



# 6) Document everything

#### TO BE DONE SHORTLY

# Bonus

# 7) Peer review

# 8) make it go live

# 9) never stop monitoring