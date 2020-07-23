# Udacity-PlagiarismDetector
Plagiarism Detector Binary Classifier developed through the Udacity Machine Learning NanoDegree

This repository contains code and associated files for deploying a plagiarism detector using AWS SageMaker.

This was an assessed project that was developed through the Udacity Machine Learning course

## Project Overview

In this project, you will be tasked with building a plagiarism detector that examines a text file and performs binary classification; labeling that file as either *plagiarized* or *not*, depending on how similar that text file is to a provided source text. Detecting plagiarism is an active area of research; the task is non-trivial and the differences between paraphrased answers and original work are often not so obvious.

## Project Outcome

A logistic regression binary classifier was selected to begin with since it has low peformance demands. On testing this showed to have high predictability ~ 96%. This is explained by the selected features having high predictability on a binary outcome: Plagiarised or Not Plagiarised.

As such, no other binary classifiers were explored.


## Directory Structure

### Data

This folder contains the corpus of text collected and created by  Paul Clough (Information Studies) and Mark Stevenson (Computer Science), at the University of Sheffield. You can read all about the data collection and corpus, at their university webpage.

Citation for data: Clough, P. and Stevenson, M. Developing A Corpus of Plagiarised Short Answers, Language Resources and Evaluation: Special Issue on Plagiarism and Authorship Analysis, In Press. 

**Notebook 2: Feature Engineering**

* Clean and pre-process the text data.
* Define features for comparing the similarity of an answer text and a source text, and extract similarity features.
* Select "good" features, by analyzing the correlations between different features.
* Create train/test `.csv` files that hold the relevant features and class labels for train/test data points.

**Notebook 3: Train and Deploy Your Model in SageMaker**

* Upload your train/test feature data to S3.
* Define a binary classification model and a training script.
* Train your model and deploy it using SageMaker.
* Evaluate your deployed classifier.

---

Please see the [README](https://github.com/udacity/ML_SageMaker_Studies/tree/master/README.md) in the root directory for instructions on setting up a SageMaker notebook and downloading the project files (as well as the other notebooks).
