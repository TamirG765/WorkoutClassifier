# Workout Classifier 🏋️‍♀️

## Introduction

This project demonstrates the process of building a deep-learning system capable of recognizing **22 different gym exercises** from short video clips. The notebook provides a step-by-step walkthrough of the entire process, from data acquisition to model training and evaluation.

## What You'll Find in the Notebook

1.  **Dataset Download & Quick Tour**:
    * Instructions on how to obtain the [*Workout Fitness Video* dataset from Kaggle](https://www.kaggle.com/datasets/hasyimabdillah/workoutfitness-video).
    * Initial inspection of the dataset, including class balance, video clip length, and example frames.

2.  **Two Preprocessing Pipelines & Model Architectures**:
    * **Frame-based Approach**:
        * Extraction of RGB frames from video clips.
        * Training of image classification models:
            * A lightweight Convolutional Neural Network (CNN).
            * A fine-tuned Vision Transformer (ViT-B/16).
    * **Pose-based Approach**:
        * Extraction of **3-D body landmarks** using MediaPipe Pose.
        * Appending per-joint velocities and confidence scores to the landmark data.
        * Feeding these sequences to custom **Multi-Stream models**:
            * ConvLSTM (Convolutional Long Short-Term Memory).
            * Transformer.

## Resources Mentioned

The notebook references several resources for further reading and understanding:
1.  [Introduction to Video Classification and Human Activity Recognition (LearnOpenCV)](https://learnopencv.com/introduction-to-video-classification-and-human-activity-recognition/)
2.  [Master Video Classification with Transformers (Medium)](https://medium.com/@iitkarthik/master-video-classification-with-transformers-train-a-hybrid-transformer-classifier-ce654e52cfc8)
3.  [Exercise\_Recognition\_AI (GitHub)](https://github.com/chrisprasanna/Exercise_Recognition_AI/blob/main/ExerciseDecoder.ipynb)
4.  [Flower Image Classification using Vision Transformer (Medium)](https://medium.com/@sanjay_dutta/flower-image-classification-using-vision-transformer-vit-50b71694cda3)
5.  [Workout Video Classifier using CNN-LSTM model (Kaggle)](https://www.kaggle.com/code/ezerelbaz/workout-video-classifier-usinng-cnn-lstm-model)

