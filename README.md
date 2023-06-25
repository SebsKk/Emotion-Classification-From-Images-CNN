# Emotion-Classification-From-Images-CNN

This project aims to create a model that can classify human emotions based on facial expressions. The model was trained on a dataset consisting of grayscale images of human faces, each labeled with one of seven emotions: anger, disgust, fear, happiness, sadness, surprise, and neutral.

## Overview
This project used a deep learning approach to solve the problem. Specifically, I used convolutional neural networks (CNN), which are particularly well-suited for image classification tasks. I also explored ensemble learning methods to combine the predictions from multiple models for improved performance.

## Data
The dataset used in this project was a collection of 48x48 pixel grayscale images of faces. The faces have been automatically registered, which means that the faces have been cropped from the original images and resized to all have the same size.

This makes the task a little simpler as the model doesn't have to deal with variation in the size and position of the faces in the images.

Each image is labeled with one of seven categories: anger, disgust, fear, happiness, sadness, surprise, and neutral.

The data was split into a training set and a testing set. Image data augmentation techniques were also applied to the training data to increase the amount and diversity of data for model training.

## Models
Several different models were trained on this task, including:

Custom-built CNN models
A reference model - a simple FNN network
For each model, I set up a pipeline that included preprocessing the image data, training the model, and then evaluating the model's performance on the test data.

Evaluation
The models were evaluated based on their accuracy on the test set. A confusion matrix was also plotted for a visual understanding of the model performance.

One interesting finding is that the ensemble of the models only outperformed the non-augmented models, but not the ones with augmentation. This is counterintuitive as ensembles usually perform at least as well as the best individual model. This outcome suggests that the models were likely making very similar mistakes, and therefore, the ensemble couldn't benefit from a diversity of predictions.

## Future Work
Some possible directions for future work on this project include:

- Experimenting with other types of models, such as different pre-trained models or different model architectures
- Applying other data augmentation techniques
- Tuning the models' hyperparameters to improve performance
