# Mask Detection
This repo contains a Mask Detection system which is built with OpenCV, Keras, TensorFlow using Deep Learning and Computer Vision concepts in order to detect face masks in static images as well as in real-time video streams.

![Python](https://img.shields.io/badge/python-v3.6+-blue.svg)


## Live Demo
[![Web Deployed version](https://www.herokucdn.com/deploy/button.svg)](https://mask-detection-web.herokuapp.com/)


## TechStack/Framework

- [OpenCV](https://opencv.org/)
- [Keras](https://keras.io/)
- [TensorFlow](https://www.tensorflow.org/)
- [Caffe-based face detector](https://caffe.berkeleyvision.org/)
- [MobileNetV2](https://arxiv.org/abs/1801.04381)

## Features
The face mask detector model is accurate, and based on MobileNetV2 architecture, it’s also computationally efficient which makes it easier to deploy the model to hardware and embedded systems like Arduino,Raspberry Pi etc.

This app can be used in real-time applications and can be integrated with embedded systems for application in railway stations, airports, schools, and public places to ensure safety in Covid-19.

## Dataset
This dataset consists of nearly __3800 images__ belonging to two labels:
*	__with_mask: 1900 images__
*	__without_mask: 1900 images__

The images used were real images of faces wearing masks. The images were collected from internet, web and kaggle.


## Installation
1. Clone the repo
```
$ git clone https://github.com/PraveenGNair/mask-detection.git
```

2. Change your directory to the cloned repo and create a Python virtual environment named 'testEnv'
```
$ mkvirtualenv testEnv
```

3. Now, run the following command in your Terminal/Command Prompt to install the libraries required
```
$ pip install -r requirements.txt
```

4. Open terminal. Go into the cloned project directory and type the following command:
```
$ python train_mask_detector.py --dataset dataset
```

5. Once the model training is completed, you would get a model file created.
Now To detect face masks in an image type the following command: 
```
$ python detect_mask_image.py --image images/pic1.jpeg
```

6. To detect face masks in real-time video streams type the following command:
```
$ python detect_mask_video.py 
```

## Streamlit app

The web app is hosted in heroku is a [Streamlit](https://streamlit.io) app  using Tensorflow & Streamlit. So to run web in local you can use below command
```
$ streamlit run app.py 
```
