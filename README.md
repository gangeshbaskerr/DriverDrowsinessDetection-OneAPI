![DRIVER_DROWSINESS_DETECTION_(CNN)-OneAPI](https://user-images.githubusercontent.com/130077430/230480144-163d76a7-6e45-4c6e-8af1-a23f26b20df8.png)
    ![made-with-jupyter-notebook](https://user-images.githubusercontent.com/130077430/230479936-93dbcbd0-275b-4af7-9231-cceeb91d8a84.svg)          ![migrated-to-oneapi](https://user-images.githubusercontent.com/130077430/230487901-cbcdf13f-1d36-477d-9a7c-1917fa579da9.svg)<img src="https://user-images.githubusercontent.com/72274851/218504609-585bcebe-5101-4477-bdd2-3a1ba13a64a8.png" width="35px"> ![built-by-team-geeks](https://user-images.githubusercontent.com/130077430/230486285-e9e8fdbc-4579-4d0e-a448-550b423199b2.svg) [![forthebadge](http://forthebadge.com/images/badges/built-with-love.svg)](http://forthebadge.com)
<img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/gangeshbaskerr/DriverDrowsinessDetection-OneAPI"> <img alt="GitHub watchers" src="https://img.shields.io/github/watchers/gangeshbaskerr/DriverDrowsinessDetection-OneAPI?style=social">
<hr/>

# Inspiration  <img src="https://user-images.githubusercontent.com/130077430/230579469-c1263cef-784e-4845-93fb-2f73544e49e1.png" width="90" height="80"> 
Accidents caused due to driver drowsiness are a major public health and safety issue, affecting millions of people every year. According to the National Safety Council, driving while drowsy is similar to driving while intoxicated, as it impairs drivers attention, reaction time, and decision making, leading to fatal or serious crashes. Several factors can increase the risk of drowsy driving, such as lack of sleep, sleep disorders, shift work, medications, and alcohol.

Research shows that driver fatigue may be a contributory factor in up to 20% of road accidents, and up to one quarter of fatal and serious accidents. An estimated 1,550 deaths, 71,000 injuries, and $12.5 billion in monetary losses are due to drowsy drivers in a year.

<img src="https://th.bing.com/th/id/OIG.WEOyPEzD_hHNRREU0GVd?pcl=1b1a19&pid=ImgGn" width="330" height="280"> <img src="https://cdn.thezebra.com/zfront/media/production/images/Have_you_ever_fallen_asleep__or__nodded_off__.width-1140.png" width="335" height="280"> <img src="https://user-images.githubusercontent.com/130077430/230591069-d29be60a-dd0c-42a9-a83b-92df7d7b03ba.gif" width="335" height="280">

<hr/>

# Introduction <img src="https://user-images.githubusercontent.com/72274851/152814876-73362bcc-bde6-411f-ba80-235e911f276f.gif" width="90" height="90">

The drowsiness detection system monitors the driver's condition and issues an alert if it detects signs of drowsiness using CNN - Python, OpenCV.

This system aims to reduce the number of accidents on the road by detecting the driver's drowsiness and warning them using an alarm⏰. 

<hr/>

# Approach <img src="https://cdn0.iconfinder.com/data/icons/data-science-2-1/66/119-512.png" width="90" height="80"> 
Here, we used Python, OpenCV, and Keras(Tensorflow) to build a system that can detect features from the face of the drivers and alert them if they ever fall asleep while driving. The system detects the eyes and prompts if it is closed or open. If the eyes are closed for 10 seconds, it will play the alarm to get the driver's attention to stop because the system has detected drowsiness. We have built a model of CNN network trained on a dataset using OneAPI that can detect closed and open eyes. Then OpenCV is used to get the live feed from the camera and run every frame through the CNN model to process it and classify whether it is opened or closed eyes.
<hr/>

# Procedure <img src="https://th.bing.com/th/id/R.02832177b40b49d50674126476f980c3?rik=aXibwvpQe645bg&riu=http%3a%2f%2fwww.clipartbest.com%2fcliparts%2fjcx%2f6rb%2fjcx6rbngi.png&ehk=xllVkMLnEE%2fEXx%2fnWbpceiVVfvTNGJmODcZ9fEBJVGA%3d&risl=&pid=ImgRaw&r=0" width="120" height="100"> 

## 1️⃣ Pre-install all the required libraries
       1) OpenCV
       2) Keras
       3) Numpy
       4) Pandas
       5) OS
## 2️⃣ Understand the dataset
       The dataset which was used is a subset of the dataset from(https://www.kaggle.com/datasets/dheerajperumandla/drowsiness-dataset)
       it has 4 folder which are
       1) Closed_eyes - having 726 pictures
       2) Open_eyes - having 726 pictures
       3) Yawn - having 725 pictures
       4) no_yawn - having 723 pictures

 <img src="https://user-images.githubusercontent.com/130077430/230722949-fa0ece8c-9d0c-45bd-b77f-863e299dd134.jpg" width="249" height="250"> <img src="https://user-images.githubusercontent.com/130077430/230722952-9b7076a0-bb3e-4be3-b102-e907fc02d030.jpg" width="249" height="250"> <img src="https://user-images.githubusercontent.com/130077430/230722954-862bbeea-9489-4b5e-8ff0-780635bd337f.jpg" width="249" height="250"> <img src="https://user-images.githubusercontent.com/130077430/230722955-f751a799-5d50-4272-bf0c-0d564a9a157e.jpg" width="249" height="250">
 
## 3️⃣ Data preprocessing
      preprocess the images from the closed_eye, open_eye, yawn and no_yawn folder and apply pre-processing techniques such as 
      normalization, resizing, and augmentation to improve the performance of the learning model.
## 4️⃣ Build and train the CNN model
<img src="https://user-images.githubusercontent.com/16632408/159187014-4bc4b70e-98d6-4313-873f-997ded2eff27.png" width="500" height="500"><img src="https://user-images.githubusercontent.com/130077430/230521431-64fbf6f1-7aca-4b67-bf67-f80a0656b784.png" width="500" height="500">
## 5️⃣ Train the model using Intel OneAPI to get better results
<img src="https://user-images.githubusercontent.com/72274851/218504609-585bcebe-5101-4477-bdd2-3a1ba13a64a8.png" width="200" height="100"><img src="https://aditech.in/wp-content/uploads/2020/07/image_2020_07_17T06_08_48_297Z.png" width="800" height="100">

**How does OneApi provide better performance :**
    
Today’s compute systems are heterogeneous and include CPUs, GPUs, FPGAs, and other accelerators. The different architectures exhibit varied                   characteristics that can be matched to specific workloads for the best performance.

Having multiple types of compute architectures leads to different programming and optimization needs. oneAPI and SYCL provide a programming model, whether through direct programming or libraries, that can be utilized to develop software tailored to each of the architectures.
    
**Advantages of using OneAPi :**

1) We can use Single code for both cpu and GPU (heterogeneous computing)
2) To implement machine learning based IoT projects easily with less hardwares as the machine learning part happens in cloud
3) To process files faster ie. it takes less time to run the epochs
4) OneAPI allows users to transcend Hardware restrictions and provide better performance for low powered computers

To migrate your project to OneAPI : 
[click here!](https://devcloud.intel.com/oneapi/get_started/) to get started
[click here!](https://www.youtube.com/watch?v=NkJXCalgmeU) for reference
    
    
## 6️⃣ Save the model
       save the model to calculate the accuracy and loss
    
<hr/>

# Accuracy and Loss      <img src="https://user-images.githubusercontent.com/130077430/230577475-9af43d03-1a50-41c2-99b2-e1a28b69c84e.png" width="90" height="80">
We did 80 epochs, to get a good accuracy from the model i.e. 98% for training accuracy and 97% for validation accuracy.
<img src="https://user-images.githubusercontent.com/130077430/230531178-35afe049-d529-452f-94a0-fe6512aa0cc6.png" width="500" height="300"> <img src="https://user-images.githubusercontent.com/130077430/230531281-573d1dbb-5200-4e09-aac4-697109e3b3ab.png" width="499" height="300">

<hr/>

# Output <img src="https://cdn4.iconfinder.com/data/icons/business-startup-36/64/552-512.png" width="90" height="80">
## Eyes opened 👀
<p align="middle"><img src="https://user-images.githubusercontent.com/130077430/230589722-bd38ad94-85a8-4ad6-9bad-675286b2d67b.gif" width="250" height="250">

## Eyes closed
<p align="middle"><img src="https://user-images.githubusercontent.com/130077430/230590473-ac7a6d4b-ed9e-4440-9a98-f65cb506482a.gif" width="250" height="250">

<hr/>

# Learnings <img src="https://user-images.githubusercontent.com/130077430/230583675-33ad7480-857b-451f-a64b-3c45f21d390a.png" width="90" height="80">
<img src="https://user-images.githubusercontent.com/72274851/218504609-585bcebe-5101-4477-bdd2-3a1ba13a64a8.png" width="200" height="100"> <img src="https://user-images.githubusercontent.com/72274851/220130227-3c48e87b-3e68-4f1c-b0e4-8e3ad9a4805a.png" width="800" height="100">
1) **Building a CNN model using Intel oneDNN :**
    oneAPI is an open-source software toolkit developed by Intel that simplifies the development of high-performance, heterogeneous applications. It allows       developers to write code that can run efficiently on a variety of architectures, including CPUs, GPUs, and FPGAs. oneDNN (Deep Neural Network) is a part     of oneAPI and is an optimized library for deep learning. It provides highly optimized building blocks for neural network models that run efficiently on a     variety of hardware platforms. 

2) **Machine Learning :**
    _How to use machine learning for identifiying the facial features from a drivers face to detect drowsiness._

3) **Convolutional Neural Network(CNN) :**
    _How to build, train and fine-tune convolutional neural networks for image and video classification._

4) **Preprocessinig the datasets :**
    _How to preprocess the data dowloaded from kaggle so that the machine learning could happen in a much better and efficient way._

5) **Different aspects of drowsiness during driving  :**
    _I have studied the different causes and reasons for drowsiness to occur and how to resolve it._
    
6) **Facial regions and drowsiness:**
    _I have studied how the facial landmarks are identified using an ocular feature called eye aspect ratio and face landmarks.Eye regions are detected           and extracted as regions of interest using a facial cue detector and The eye aspect ratio values are then calculated, analyzed and saved for each image._
    
7) **Team work :**
    _Collaborating and communicating effectively in a team to deliver a project._

8) **Understanding the need for a drowsiness detection system in vehicles**

_These are just a few examples of the knowledge and skills that i likely gained while building this project. Overall, building a drowsiness detection model  is a challenging and rewarding experience that requires a combination of technical expertise and knowledge on facial cue detection._

<hr/>

# Project Deployment <img src="https://user-images.githubusercontent.com/130077430/230725195-2f024fca-9cae-4e91-85dc-4c12e0e1fcb0.png" width="90" height="80">

We have built an app using Flutter. Flutter helps Build, test, and deploy beautiful mobile, web, desktop, and embedded apps from a single codebase. It is a cross-platform app development framework by Google which goes hand in hand with the model to help ensure the safety of the user and other commuters. 

As soon as the model detects drowsiness, the model will send an API request call to the client app, which notifies the user to take some rest and shows the navigation option to the nearest resting places. If the user isn't drowsy, the app will give 10 seconds buffer time within which the user can confirm that he isn't sleepy by pressing the prompt on the screen. If the user is drowsy he will get a option for getting driving assistance from the nearby driving service providers. If the user has been detected drowsy more than three times within 10 minutes, a notification is sent to the highway patrol and the nearby drivers as a concern for the safety of other drivers and the drowsy driver.


<img src="https://user-images.githubusercontent.com/130077430/230727293-bd42e1a8-29cb-4114-841c-64578c4bd0ca.png" width="250" height="500"><img src="https://user-images.githubusercontent.com/130077430/230726528-77ba9f99-bb0c-40f8-87d0-c764bf270ae0.png" width="250" height="500"><img src="https://user-images.githubusercontent.com/130077430/230726528-77ba9f99-bb0c-40f8-87d0-c764bf270ae0.png" width="250" height="500"><img src="https://user-images.githubusercontent.com/130077430/230726528-77ba9f99-bb0c-40f8-87d0-c764bf270ae0.png" width="250" height="500">

<hr/>

# One more thing <img src="https://cdn.freebiesupply.com/logos/large/2x/apple1-logo-png-transparent.png" width="60" height="60">
<p align="middle"><img src="https://th.bing.com/th/id/R.cfabfe3a83a918b326ede9efb1d7ee8b?rik=sxInqysclnUS1A&riu=http%3a%2f%2fmedia.idownloadblog.com%2fwp-content%2fuploads%2f2015%2f08%2fSteve-Jobs-One-More-Thing.jpg&ehk=VbXo3DNGszgubtTtwYXhvwQyxwDKVJ%2bW7%2b0%2bproDQ%2fM%3d&risl=&pid=ImgRaw&r=0" width="800" height="300">

1) **Distraction detection :**
    When no eyes is detected while face is detected, It can be called distraction and that can also be added to this model. 

2) **Alcohol gas detection :**
    The MQ3 alcohol gas sensor is a module used for detecting alcohol, CH4, benzene, gasoline, hexane, CO, and LPG. It has a sensitive material namedSnO2 for     alcohol gas detection, This code can be easily pared with MQ3 sensor to extend its detection in drunken driving.

3) This module can be integrated with the driving system in cars to slow them down and bring them to stop when drowsiness is detected, its even better with      autonomous cars as they can take over the driver and park the car in a safe place and prompt the driver to rest for few hours and then continue their        journey.

<hr/>
