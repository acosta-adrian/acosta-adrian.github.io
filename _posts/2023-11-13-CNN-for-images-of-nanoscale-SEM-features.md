---
layout: post
title:  "Convolutional neural network trained on nanoscale SEM features"
date:   2023-11-13 15:29:10
blurb: "Convolutional neural network trained on nanoscale SEM features"
og_image: /assets/img/image.png
---

<img src="{{ "/assets/img/image_2.png" | absolute_url }}" alt="demo of CNN model" class="post-pic"/>

Link to Kaggle notebook for this project: https://www.kaggle.com/code/adrianacosta0/cnn-for-images-of-nanoscale-sem-features?scriptVersionId=157256158

In this project, I explored the application of Convolutional Neural Networks (CNNs) to classify nanoscale features in Scanning Electron Microscope (SEM) images. 

I started with a public set of SEM images of nanoscale features already categorized into various classes based on their features, such as particles, powder, biological structures, nanowires, and more. I sourced this dataset from here: https://www.nature.com/articles/sdata2018172

The goal was to develop a supervised ML model that could automatically categorize SEM images into these prelabeled categories.

The approach involved the following steps:

    1. Data Preprocessing: The SEM images were preprocessed, this included cropping/resizing the images and splitting them into training, validation, and test sets.

    2. Model Building: I used the InceptionV3 architecture as the base model, freezing those layers, then added a single layer on top for the specific classification task. The model was compiled with the Adam optimizer and categorical crossentropy loss function.

    3. Model Training: The model was trained on the training set, with validation performed on the validation set to monitor the model's performance and prevent overfitting.

    4. Evaluation: The trained model was evaluated on the test set to assess its accuracy in classifying SEM images. Additionally, a confusion matrix and classification report were generated to provide insights into the model's performance across different classes.

    5. Testing on External Data: To further validate the model's generalizability, it was tested on a separate dataset of SEM images not used in the training or validation process. This helped to assess how well the model could perform in real-world scenarios. I took these images from various wikipedia articles that I found that had SEM images.

The trained model showed >90% accuracy classifying SEM images on both the test set and external data. 
