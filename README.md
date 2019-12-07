## OpenPose-Visualizer
> Vanderbilt *CS3891* *Introduction to Visualization* Final Project, fall 2018
> 
> I would like to thank Professor *Matthew Berger* and Professor *Benoit Dawant* for their help and guidance on this project
> 

#### Contents
- [Description](#description)
- [Overview](#overview)
- [Setup](#setup)
- [Process Book](#process-book)
    - [Motivation and Goals](#motivation-and-goals)
    - [Initial Data Analysis](#initial-data-analysis)
    - [Data Cleaning Process](#data-cleaning-process)
    - [Visualization Features](#visualization-features)
    - [Implementation Overview](#implementation-overview)
    - [Final Product](#final-product)
- [Feedback and Evaluations](#feedback-and-evaluations)

### Description
The motivation of the *OpenPose Visualizer Project* is to build a visualization tool for constructing a proof-of-concept for designing an autonomous system that monitors the movements of epilepsy patients and uses machine learning algorithms to predict the onset of a potential epilepsy episode. We speculate that there are certain *movement patterns* that are likely to be indicators of a potential epilepsy episode and thus we should be able to train a neural network to recognize such patterns.
Using *OpenPose*, we are able to identify and record the positions of various keypoints on a human body. However, it is hard for us to analyse and evaluate the validity of these data. Therefore, the OpenPose Visualizer aims to represent these data in a way that is intuitive and effective to the human eyes, thus making it possible for us to get a better understanding of the data.

### Overview
The *OpenPose Visualizer* used **[d3.js](https://d3js.org/)** to visualize and interact with the data.
File [`Documents`](/Documents) includes the proposal, process book and other related document files of the project; [`Data`](/Data) includes the raw data as well as the processed data used in this project. It also includes the python script used for the processing; [`Source`](/Source) contains all of the project code.


### Setup
To run the project, clone the project repository to your local machine and run `python -m SimpleHTTPServer` in the terminal in the root directory of the project. Then, go to the following url: [http://localhost:8000/](http://localhost:8000/) in your browser to see the project contents.

---

## Process Book

### Motivation and Goals
As mentioned above, the motivation of the *OpenPose Visualizer Project* is to build a visualization tool for constructing a proof-of-concept for designing an autonomous system that monitors the movements of epilepsy patients and uses machine learning algorithms to predict the onset of a potential epilepsy episode. We want the visualization to help us gain a better understanding of the following questions:
1. Are the data generated by *OpenPose* accurate enough for us to reconstruct the movement trace?
2. If so, are there any movement patterns distinct enough for the human eyes to recognize during an epilepsy episode?
3. If so, can we use these patterns as indicators of a potential epilepsy episode?

### Initial Data Analysis
A detail overview of the data generated by the *OpenPose* can be found [here](https://github.com/CMU-Perceptual-Computing-Lab/openpose/blob/master/doc/output.md). I wrote a few python scripts to calculate the Euclidean distance of the same keypoint position between every two consecutive frames for each keypoint in the original JSON file and combine the results into one single JSON file. Given the timeline and data validity (*OpenPose* did not recognize the patient’s face for most of the frames due to the quality of the video), the *OpenPose Visualizer* will only be using the data from [pose_keypoints_2d](/Data/EMU_Processed/pose_keypoints_2d.json), [hand_left_keypoints_2d](/Data/EMU_Processed/hand_left_keypoints_2d.json), and [hand_right_keypoints_2d](/Data/EMU_Processed/hand_right_keypoints_2d.json).

### Visualization Features
## 11/10/2019

## 11/14/2019

## 11/18/2019

### Implementation Overview
## 11/10/2019

## 11/14/2019

## 11/18/2019

### Final product

---

### Feedback and Evaluations

