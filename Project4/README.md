# Project: Motion Compensated Pulse Rate Estimation

## Introduction
This project has 2 main parts.

Develop a Pulse Rate Algorithm on the given training data. Then Test Your Algorithm and see that it has met the success criteria.
Apply the Pulse Rate Algorithm on a Clinical Application and compute more clinically meaningful features and discover healthcare trends.

A core feature that many users expect from their wearable devices is pulse rate estimation. Continuous pulse rate estimation can be informative for many aspects of a wearer's health. Pulse rate during exercise can be a measure of workout intensity and resting heart rate is sometimes used as an overall measure of cardiovascular fitness. In this project you will create a pulse rate estimation algorithm for a wrist-wearable device. Use the information in the Physiological Mechanics of Pulse Rate Estimation section below to inform the design of your algorithm. Make sure that your algorithm conforms to the given Algorithm Specifications in the following concept, Part 1: Overview & Instructions.

## Algorithm Specifications
You must build an algorithm that:

- estimates pulse rate from the PPG signal and a 3-axis accelerometer.
- assumes pulse rate will be restricted between 40BPM (beats per minute) and 240BPM
- produces an estimation confidence. A higher confidence value means that this estimate should be more accurate than an estimate with a lower confidence value.
- produces an output at least every 2 seconds.


## Dataset
You will be using the Troika dataset to build your algorithm. Find the dataset under datasets/troika/training_data. The README in that folder will tell you how to interpret the data. The starter code contains a function to help load these files.

Zhilin Zhang, Zhouyue Pi, Benyuan Liu, ‘‘TROIKA: A General Framework for Heart Rate Monitoring Using Wrist-Type Photoplethysmographic Signals During Intensive Physical Exercise,’’IEEE Trans. on Biomedical Engineering, vol. 62, no. 2, pp. 522-531, February 2015. Link

## Environment Setup
For step by step instructions on creating your environment, please go to https://github.com/udacity/nd320-c4-wearable-data-starter

