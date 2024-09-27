
# Face Detection System

## Table of contents
- [Introduction](#introduction)
- [What is Face Detection?](#whatisfacedetection?)
- [Project Structure](#projectstructure)
- [Features](#features)
- [Conclusions](#conclusions)
- [Documentation](#documentation)
- [Contributors](#contributors)

## Introduction

This project aims to develop a face detection system capable of identifying human faces in an image. As an educational project, the model is trained from scratch without relying on pre-trained models. The system is designed to operate under computational constraints, making efficient use of available resources.

## What is Face Detection?

Face Detection is a branch of Computer Vision (CV) focused on identifying human faces within images. Due to the growing availability of digital images, face detection plays a crucial role in various fields and applications. Historically, techniques such as the Viola-Jones algorithm have been used for this purpose. However, modern approaches often rely on deep learning, which, while effective, requires significant computational resources to train from scratch.

Considering the constraints of this project—namely, the need to train a model from scratch and the absence of significant computational resources—we have opted to use a Support Vector Machine (SVM) in combination with feature extraction techniques for classification. This approach is paired with algorithms capable of locating faces regardless of position and size within the image.

## Project Structure

The notebook is organized into the following sections:

1. **Dataset Construction**: How the dataset was built for training and testing.
2. **Feature Extraction**: Methods used to extract relevant features from images (HOG, LBP, LBPH).
3. **Model Training and Testing**: Selection, training, and testing of the SVM classifier.
4. **Face Detection Algorithm**: Implementation of the face detection algorithm, tested on real-world photos.

## Features
- Feature extraction techniques to improve the efficiency of the classifier.
- Face classification using a custom-trained Support Vector Machine (SVM).
- Face detection algorithms to localize faces regardless of size and position.
- Test results on real-world photos.
  
## Conclusion
The trained SVM classificator performed very well in face classication task, with an accurcy score of 0.99 on the test set. Thanks to the implemented sliding window and image pyramids and Non-maximum Suppression (NMS) algorithms, the model was able to identify most of the faces in test photos.
The project also includes examples of the face detection algorithm applied to real-world photos, demonstrating the effectiveness of the SVM classifier and feature extraction methods.


## Documentation

For a detailed explanation of the methods and algorithms used, refer to the following resources:

- [Face detection techniques: a review](https://link.springer.com/article/10.1007/s10462-018-9650-2)
- [Human Face Detection Techniques: A Comprehensive Review and Future Research Directions](https://www.mdpi.com/2079-9292/10/19/2354)
- [Review and Comparison of Face Detection Techniques](https://link.springer.com/chapter/10.1007/978-981-15-0361-0_1)
- [Face Detection Explained: State-of-the-Art Methods and Best Tools](https://medium.com/sciforce/face-detection-explained-state-of-the-art-methods-and-best-tools-f730fca16294)
- [What is Face Detection? Ultimate Guide 2023 + Model Comparison](https://learnopencv.com/what-is-face-detection-the-ultimate-guide/)
- [Histogram of Oriented Gradients and Object Detection](https://pyimagesearch.com/2014/11/10/histogram-oriented-gradients-object-detection/)
- [Image Classification using HOG and LBP Feature Descriptors with SVM and CNN](https://www.ijert.org/image-classification-using-hog-and-lbp-feature-descriptors-with-svm-and-cnn)
- [Understanding the Local Binary Pattern (LBP): A Powerful Method for Texture Analysis in Computer Vision](https://aihalapathirana.medium.com/understanding-the-local-binary-pattern-lbp-a-powerful-method-for-texture-analysis-in-computer-4fb55b3ed8b8)
- [Face Recognition: Understanding LBPH Algorithm](https://towardsdatascience.com/face-recognition-how-lbph-works-90ec258c3d6b)
- [DIP 07 - Image Description (4) - Texture analysis with LBP implemenation in python and skimage](https://www.youtube.com/watch?v=_5ktOnEZ3O4&t=309s)
- [Sliding Windows for Object Detection with Python and OpenCV](https://pyimagesearch.com/2015/03/23/sliding-windows-for-object-detection-with-python-and-opencv/)
- [Image Pyramids with Python and OpenCV](https://pyimagesearch.com/2015/03/16/image-pyramids-with-python-and-opencv/)
- [Non-maximum Suppression (NMS)](https://towardsdatascience.com/non-maximum-suppression-nms-93ce178e177c)
- [Non-Maximum Suppression for Object Detection in Python](https://pyimagesearch.com/2014/11/17/non-maximum-suppression-object-detection-python/)



## Contributors
- [Francesco Gardini](https://github.com/gardi97)
