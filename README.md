# Face-Recognition-System

### Face Recognition using Haar-Cascade Classifier, OpenCV and Python. 

[![Generic badge](https://img.shields.io/badge/Face-Recognition-blue.svg?style=for-the-badge)](https://github.com/jashan20/Face-Recognition-System) 
[![Generic badge](https://img.shields.io/badge/Open-CV-orange.svg?style=for-the-badge)](https://github.com/jashan20/Face-Recognition-System) [![Generic badge](https://img.shields.io/badge/HaarCascade-Classifier-teal.svg?style=for-the-badge)](https://github.com/jashan20/Face-Recognition-System)

This project is based on face detection and face recognition processes. It is a real time web cam face detection and recognition project which will be used to generate training face images and then detect the known faces. It classifies between known and unknown faces.


## Requirements
- Python 3.5
- OpenCV 3.1.0
- Numpy

## Outline

[![Made with Python](https://forthebadge.com/images/badges/made-with-python.svg)](https://github.com/jashan20/Face-Recognition-System) [![Built with love](https://forthebadge.com/images/badges/built-with-love.svg)](https://github.com/jashan20) [![4U](https://forthebadge.com/images/badges/for-you.svg)](https://github.com/jashan20/Face-Recognition-System) 

This project consist of 3 parts, which are:

1. Creating datasets (**facedata.py**)
2. Train the model (**facedata.py**)
3. Recognize faces (**facerecognition.py**)

#Steps for create dataset and train the model
1. Read and show video stream, capture images
2. Detect Faces and show bounding box (haarcascade)
3. Flatten the largest face image(gray scale) and save in a numpy array
4. Repeat the above for multiple people to generate training data

#Steps for recognize faces using **KNN** algorithm
1. load the training data (numpy arrays of all the persons)
		 x- values are stored in the numpy arrays
		 y-values we need to assign for each person
2. Read a video stream using opencv
3. extract faces out of it
4. use knn to find the prediction of face (int)
5. map the predicted id to name of the user 
6. Display the predictions on the screen - bounding box and name
