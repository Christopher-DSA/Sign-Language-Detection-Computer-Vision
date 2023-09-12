# Sign-Language-Detection-Computer-Vision

## Introduction

The goal is to create a fast and accurate system that uses a webcam to recognize sign language in real-time. 


The motivation is to explore the tensorflow machine learning libary and apply it to a practical application.

## Table of Contents

1. [Introduction](#introduction)
2. [Features](#features)
3. [Tech Stack](#tech-stack)
4. [Installation](#process)
5. [Future Work](#future-work)

## Features
-Can distinguish between four sign language gestures in real-time (Hello, Thank you, Yes, No)

-Lightweight and speedy object detection (SSD mobile net 300x300 base network)

-Can detect multiple hands at once.

## Tech Stack
- Python 3.9
- OpenCV
- TensorFlow
- Label-Studio

## Process
1. Creating a vitrual anaconda enviroment using python 3.9 for the project.
2. Creating a script to automatically collect photos for the dataset.
3. Importing the collected images into label-studio for annotation.
4. Downloading the ```ssd_mobilenet_v2_fpnlite_320x320_coco17_tpu-8``` object detection model.
5. Setting up the model config for transfer learning.
6. Training the model.
7. Use open-cv to capture frames from the webcam.
8. Use tensorflow to convert the image into a tensor for the model.
9. Preform sign detection.
10. Show result on screen using open-cv to draw a label/bounding box on the screen.
   

## Future Work
-Train the object detection model with more signs.
-Create a GUI for the program. So users can select which signs the would like to practice.
-Explore alternate techniques for solving this problem such as Google Mediapipe (computer vision framework).
