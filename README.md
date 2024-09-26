# Gesture Recognition Assignment
> As a data scientist at a home electronics company which manufactures state of the art smart televisions. You want to develop a cool feature in the smart-TV that can recognise five different gestures performed by the user which will help users control the TV without using a remote. The gestures are continuously monitored by the webcam mounted on the TV. Each gesture corresponds to a specific command:
- Thumbs up:  Increase the volume
- Thumbs down: Decrease the volume
- Left swipe: 'Jump' backwards 10 seconds
- Right swipe: 'Jump' forward 10 seconds  
- Stop: Pause the movie

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- Poblem Statement: To build a Deep Learning model which can recognize the gestures. 
- The training data consists of a few hundred videos categorised into one of the five classes. 
- Each video (typically 2-3 seconds long) is divided into a sequence of 30 frames(images). These videos have been recorded by various people performing one of the five gestures in front of a webcam - similar to what the smart TV will use. 
- The data is in a zip file. The zip file contains a 'train' and a 'val' folder with two CSV files for the two folders. These folders are in turn divided into subfolders where each subfolder represents a video of a particular gesture. Each subfolder, i.e. a video, contains 30 frames (or images).
- All images in a particular video subfolder have the same dimensions but different videos may have different dimensions. 
- Each row of the CSV file represents one video and contains three main pieces of information - the name of the subfolder containing the 30 images of the video, the name of the gesture and the numeric label (between 0-4) of the video.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- Built multiple models using different statergies to find out the best model to solve the problem statment.
- Experiments were performed with Conv3D, Conv2D+GRU, Conv2D+LSTM, MobileNet Model, along with statergies like Scaling, Dropouts, Data Augmentation, Batch Normalization Statergies helped building a good model.
- The Transfer Learning model is deemed to be the best model.
- Models bulit performed better when Scaling, Dropouts, Normalizations, Adding Layers were useful.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Technologies Used
- numpy - 1.26.4
- pandas - 2.2.2
- matplotlib - 3.7.5
- tensorflow - 2.15.0

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
- This project took help from on [this tutorial](https://www.tensorflow.org/tutorials/images/classification).

## Contact
Created by [@tritammohanty](https://github.com/tritammohanty) - feel free to contact me!

<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
