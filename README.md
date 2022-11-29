# AI FOR HEALTHCARE-Nanodegree Project

## Project 1: Pneumonia Detection from Chest X-Rays

In this project, you will apply the skills that you have acquired in this 2D medical imaging course to analyze data from the NIH Chest X-ray Dataset and train a CNN to classify a given chest x-ray for the presence or absence of pneumonia. This project will culminate in a model that can predict the presence of pneumonia with human radiologist-level accuracy that can be prepared for submission to the FDA for 510(k) clearance as software as a medical device. As part of the submission preparation, you will formally describe your model, the data that it was trained on, and a validation plan that meets FDA criteria.

- [Link to project](https://github.com/nguyenduchuyvn/AI-FOR-HEALTHCARE-Udacity/tree/main/Project1)

## Project 2: Hippocampal Volume Quantification in Alzheimer's Progression
In this project you will build an end-to-end AI system which features a machine learning algorithm that integrates into a clinical-grade viewer and automatically measures hippocampal volumes of new patients, as their studies are committed to the clinical imaging archive.

Fortunately you won't have to deal with full heads of patients. Our (fictional) radiology department runs a HippoCrop tool which cuts out a rectangular portion of a brain scan from every image series, making your job a bit easier, and our committed radiologists have collected and annotated a dataset of relevant volumes, and even converted them to NIFTI format!

You will use the dataset that contains the segmentations of the right hippocampus and you will use the U-Net architecture to build the segmentation model.

After that, you will proceed to integrate the model into a working clinical PACS such that it runs on every incoming study and produces a report with volume measurements.

- [Link to project](https://github.com/nguyenduchuyvn/AI-FOR-HEALTHCARE-Udacity/tree/main/Project2)

## Project 3: Patient Selection for Diabetes Drug Testing
EHR data is becoming a key source of real-world evidence (RWE) for the pharmaceutical industry and regulators to make decisions on clinical trials. You are a data scientist for an exciting unicorn healthcare startup that has created a groundbreaking diabetes drug that is ready for clinical trial testing. It is a very unique and sensitive drug that requires administering the drug over at least 5-7 days of time in the hospital(X number of days based off of distribution that I will see in data and cutoff point) with frequent monitoring/testing and patient medication adherence training with a mobile application. You have been provided a patient dataset from a client partner and are tasked with building a predictive model that can identify which type of patients the company should focus their efforts testing this drug on. Target patients are people that are likely to be in the hospital for this duration of time and will not incur significant additional costs for administering this drug to the patient and monitoring.

In order to achieve your goal you must first build a regression model that can predict the estimated hospitalization time for a patient and also provide an uncertainty estimate range for that prediction so that you can rank the predictions based off of the uncertainty range.


- [Link to project](https://github.com/nguyenduchuyvn/AI-FOR-HEALTHCARE-Udacity/tree/main/Project3)
