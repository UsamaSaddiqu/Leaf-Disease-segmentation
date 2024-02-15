# Leaf-Disease-segmentation
A deep learning project for segmenting diseases in plant leaves. Utilizes UNet architecture with EfficientNetB3 as backbone for accurate segmentation.

**Plant Leaf Disease Segmentation**

This repository contains a project for segmenting diseases in plant leaves using deep learning techniques. The dataset used in this project is sourced from Kaggle, consisting of 2940 images of diseased leaves along with their corresponding masks. The data collection is based on the PlantDoc images. There are no train test splits.


**Dataset Details**

The dataset consists of images depicting various plant leaf diseases such as Apple Scab Leaf, Apple rust leaf, Bell pepper leaf spot, Corn leaf blight, Potato leaf early blight, among others. Each image is accompanied by a mask containing both the background and the diseased regions.

**Project Overview**

In this project, we utilized Keras for implementation. The main steps involved:

**Dataset Loading and Preprocessing:** 

Two classes were defined for loading and preprocessing the dataset. Due to variations in image dimensions, they were standardized to (160,160). Images were read in RGB format using OpenCV.

**Data Splitting:** 

The dataset was split into training, validation, and test sets using a ratio of 70:15:15, respectively.

**Model Architecture:** 

The UNet architecture with EfficientNetB3 as the backbone was employed for disease segmentation.

**Loss Function:** 

Two loss functions were used for optimization:

Dice Loss

Binary Focal Loss

The total loss was calculated as a combination of the two.

**Training:** 

The model was trained for 10 epochs with a batch size of 8. Achieved metrics include:

**Training Accuracy:** 96.93%

**Validation Accuracy:** 92.65%

**Training loss:** 0.0446

**Validation loss:** 0.1101

**Test loss:** 0.1528

**Training IoU Score:** 0.9626

**Validation IoU Score:** 0.9121

**Test IoU Score:** 0.9059

**Training F1 Score:** 0.9809

**Validation F1 Score:** 0.9524

**Test F1 Score:** 0.8746

**Evaluation:**

Predicted segmented masks were overlaid on test images for visual assessment. Some of the predicted masks along with original images and ground truths are also attatched.

**Inspiration for project:**

This project aims to address the challenge of detecting diseases in plant leaves through image segmentation, potentially aiding in early disease diagnosis and crop management strategies.

Feel free to explore the code and experiment further! Your contributions and feedback are welcome.

**Note:** Please ensure to comply with the dataset's licensing terms and conditions before usage.

**Acknowledgements**
Special thanks to the creators of the PlantDoc dataset for providing valuable resources for research and development in plant disease detection.


