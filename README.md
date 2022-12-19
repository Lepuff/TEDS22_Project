# TEDS22_Project
## Introduction

This repoistory contains the code for a project in the course Embedded and distributed AI at jönköking University.

The aim of the project is to create a embedded AI application for object detection on an edge device. In this specific project we have choosen to work with an android device.

The project is done by the following students.
* Emil Christoffersson
* Philip Djup
* Oskar Persson
* Samuel Svensson



## Usage

The app is simple to use. When the app is run for the first time, permissions for the camera needs to be accepted. When the app is opened, the camera will start and the user can point the camera at objects in the world. The app will then try to detect what object is in the image and display the result. The app can detect 91 different objects.

## Model 

In this project, a compressed TensorFlow Lite (TFLite) version of MobileNetV1 in Android Studio to develop a mobile application was used.
The efficient architecture and low computational requirements of MobileNetV1 allowed for the creation of a fast and responsive app.
The goal of the project was to create a user-friendly app that could perform object detection tasks on a mobile device in real-time, utilizing the power of TFLite and MobileNetV1 to deliver high-quality results. 

The model was trained on the Coco-SDD dataset. The dataset contains images of objects that are normally encountered in everyday life covering  11 superclasses and 91 distinct categories.
 The images are scenes or situations that contain these objects. The dataset contains 328,000 images with a total of 2.5 million labeled instances. 

## Development
Devlopment was done using Android studio 2021.3.1 Patch 1, using the following plugins and implementations:

* androidx.core:core-ktx:1.7.0 
* androidx.appcompat:appcompat:1.5.1
* implementation  com.google.android.material:material:1.7.0 
* androidx.constraintlayout:constraintlayout:2.1.4 
* androidx.lifecycle:lifecycle-viewmodel-ktx:2.4.0 
* org.tensorflow:tensorflow-lite-support:0.1.0 
* org.tensorflow:tensorflow-lite-metadata:0.1.0 
* androidx.camera:camera-camera2:1.0.0-beta10
* androidx.camera:camera-lifecycle:1.0.0-beta10
* androidx.camera:camera-view:1.0.0-alpha17"
* androidx.activity:activity-ktx:1.1.0"
* org.tensorflow:tensorflow-lite-gpu:2.3.0 

### Requirements

The app requries permission to the camera as well as an Android SDK version 21.0 or higher translating to Android version 5.0 or higher.

### Build from source
To build the app from source, clone the repository and open it in Android Studio. Then build the app using the build button in Android Studio.