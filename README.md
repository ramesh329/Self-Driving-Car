
# Building a end-to-end model of a Self-Driving Car Using CNN

## Problem Statement :
Given the 25-min video which is broken down into 30 Frames per second(one image per 2 milli-seconds) from a front-camera of     Car and corresponding steering angles in degrees , we need to train a model that predicts the steering angle based on the input image.
    

## Constraints :
   * Here we considering only steering angle as target variable, in real scenarios we need to consider breaking ,accelerator,
   usage of whipers and signal indicators
   * We assume that car is equiped with automatic transmission (changing clutch and gear automatically but not manually)
   * We also have not considered basic rules of Traffic to avoid collisons
   

## About Data :
    It's a 25-min recorded video which is broken down into images and correspoding steering angles recorded in data.txt file

    Dataset: https://github.com/SullyChen/Autopilot-TensorFlow
            [https://drive.google.com/file/d/0B-KJCaaF7elleG1RbzVPZWV4Tlk/view]
    Size: 25 minutes = 25*60*30 = 45,000 images ~ 2.3 GB
 
 **Note:** 
     * Here the steering angles are in degress , so we need to convert them into radians
     * Spliting of Data happens in a temporal way, first 70%  of the data as train and rest as test
     * we take last 150 rows of a image to avoid unnecessary things like sky etc and for faster training of the model
