# Title: Automated Cardiac Segmentation for Medical Analysis

### Short Summary: For the capstone computer science class CISC 4900, I decided to do a pure machine learning project on cardiac segmentation.


## Introduction

### Understand What The Heart Is
The heart is a muscular organ responsible for pumping blood throughout the body, delivering oxygen and nutrients to tissues and organs while removing waste products. 
It consists of four chambers: the left and right atria, which receive blood from the body and lungs respectively, and the left and right ventricles, which pump blood to the body and lungs respectively. 
The heart also contains valves that regulate the flow of blood between its chambers and major blood vessels.

### What Is Segmentation:
Typically when a patient has heart complications, medical professionals (usually cardiologists) order that the patient gets a range of imaging done on their heart. 
After this, a medical imaging specialist segments the images to isolate the heart or its muscles so that the doctor or cardiologist can use the images to plan treatments. 
The segmentation involves separating structures around the heart and from the heart so that a doctor can just look at the images and plan for the patient. 
This process, however, of segmenting the cardiac structures takes time and is just now starting to be automated with machine learning. 
By being able to segment a patient's organs faster and with accuracy, heart specialists can spend more time planning for the treatment of their patient because they can see their patient's heart. [^1]

### My Objective:
The goal of this project is to make and evaluate a machine-learning model for automated segmentation from cardiac magnetic resonance imaging (MRI). [^2]
The model would be able to accurately segment the cardiac structures like left atrium, right atrium, left ventricle, right ventricle, and myocardium to enable a heart specialist to better diagnose and treat their patient.

### Methodology:
1. Obtain a dataset for training, validation, and testing [^2]
2. Preprocess the data. Account for color, and image resolution and normalize their values.
3. Either design a convolutional neural network that uses the u-net schema or (very likely) use transfer learning
4. Train the model using the annotated dataset, employing techniques such as data augmentation, transfer learning, and fine-tuning to enhance generalization
5. Evaluate the performance of the trained model using quantitative metrics, including Dice similarity coefficient (DSC) and Hausdorff distance
6.  Validate the generalizability and clinical utility of the automated segmentation framework using an independent test set from some set the model has never seen
7.  Attempt to make the model into a usable tool where a user can input an image, and the model will be able to segment the image accurately 



[^1]: Haq, R., Hotca, A., Apte, A., Rimner, A., Deasy, J. O., & Thor, M. (2020). 
Cardio-pulmonary substructure segmentation of radiotherapy computed tomography images using convolutional neural networks for clinical outcomes analysis. 
Physics and Imaging in Radiation Oncology, 14, 61–66. https://doi.org/10.1016/j.phro.2020.05.009
[^2]: The datasets I will be using are from a publicly available dataset. https://www.cardiacatlas.org/sunnybrook-cardiac-data/