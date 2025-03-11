# Final project: Coral Object Detection
This project showcases the experimentation of YOLO (You Only Look Once) as a state-of-the-art real-time object detection system that stands out for its real-time capabilities. The dataset used consists of custom data obtained from a collection of coral reef images gathered during a survey conducted by a Remotely Operated Underwater Vehicle (ROV). Subsequently, the data was manually annotated in Roboflow. The model has been trained to fulfill the requirements of detecting coral life forms for analyzing the impact of climate change on coral biodiversity in a marine survey area.
https://docs.google.com/presentation/d/11uNN066W8HUieTp2LAaC45LjVdw8UQi4utRGyHKmEvU/edit#slide=id.g26793589b75_0_208

* Project's title: **Coral Life Forms Detection for Analysis of Climate Change Impact on Coral Biodiversity**
* Authors: Hilmy Rahmadani
  
📝 Note: This is a final project of the Computer Vision Bootcamp by PT Teknologi Artifisial Indonesia (IndonesiaAI).

## ★ Introduction

### Background

Coral reefs, often referred to as the "rainforests of the sea," are some of the most diverse ecosystems in the world. Thousands of species rely on reefs for survival. Millions of people all over the world also depend on coral reefs for food, protection and jobs. Unfortunately, these vital ecosystems are facing unprecedented threats due to climate change.

[National Oceanic and Atmospheric Administration (NOAA)](https://oceanservice.noaa.gov/facts/coralreef-climate.html) stated that climate change will affect coral reef ecosystems, through sea level rise, changes to the frequency and intensity of tropical storms, and altered ocean circulation patterns. When combined, all of these impacts dramatically alter ecosystem function, as well as the goods and services coral reef ecosystems provide to people around the globe.

Traditional methods of coral assessment, such as Line Intercept Transect (LIT) for identifying coral coverage, often face limitations in terms of scope and efficiency. These limitations are particularly evident in survey scalability and the constraints of human diving time. To bridge this gap, our project is dedicated to the utilization of automatic Coral Life Forms Detection for conducting a comprehensive analysis of coral coverage during site surveys by a Remotely Operated Underwater Vehicle (ROV).

By integrating cutting-edge detection techniques into an automated coral monitoring method using an underwater robot, our objective is to offer a more nuanced understanding of how climate change impacts various coral species, their distribution, and overall reef dynamics. This endeavor aims to empower researchers and conservationists to make decisions about further interventions more efficiently. 

### Project objective & scope

**Objective :**
Develop deep learning models for identifying and analyzing coral life forms, focusing on seven main forms (Branching, Massive, Submassive, Foliose, Mushroom, Tabulate, Encrusting).

**Scope :**
Explore YOLO state of the art object detection algorithm in developing deep learning model for coral life forms detection.
  
## ★ Getting Started

### 1. Data collection & Preparation

### 🔍 Dataset : [Coral Life Forms Detection](https://universe.roboflow.com/computer-vision-xiyu1/coral-life-forms-detection/dataset/3)

<img align="left" src="https://github.com/triwahyupra/project-coral-monitoring/blob/6bfd0463506ee3eecb6f7b5e107ce5bf7a68b7b0/assets-finalproject/roboflow-custom-dataset.png" alt="LOGO" width="250" height="200">
The data is collected through video extraction recorded by a Remotely Operated Underwater Vehicle (ROV) conducting surveys of coral reefs at depths ranging from 8 to 15 meters underwater in the North Bali Sea, specifically in the coastal area of Les village, Buleleng Regency, Bali, Indonesia. The extracted images then proceed to undergo manual annotation into seven distinct classes within Roboflow, enabling a detailed classification of coral life forms.
  
```
class_names = ['Branching', 'Encrusting', 'Foliose', 'Massive', 'Mushroom', 'Submassive', 'Tabulate']
num_classes = 7
```  
**Data Split :**

<img align="center" src="https://github.com/triwahyupra/project-coral-monitoring/blob/6bfd0463506ee3eecb6f7b5e107ce5bf7a68b7b0/assets-finalproject/original-data-split.png" alt="original" width="630" height="100">

Preprocess and add augmentation on train set to increase data variation :
Preprocessing | Augmentation 
:-----:|:----------:
Auto-Orient | Flip (Horizontal, Vertical)
Resize (640x640) | Grayscale (15%)
. | Hue (+/- 15°)

<img align="center" src="https://github.com/triwahyupra/project-coral-monitoring/blob/6bfd0463506ee3eecb6f7b5e107ce5bf7a68b7b0/assets-finalproject/augmented-data-split.png" alt="augmented" width="630" height="100">

### 2. Model Development

### YOLO (You Only Look Once)

Examining and Compare the architectural variations of **YOLOv3u**, **YOLOv5s**, and **YOLOv8s** to optimize the accuracy and efficiency of the coral life form detection system.

Initializing Hyperparameters :
```
Epoch :100
Batch_size : 16
Img_size : 416
lr0 = 0.01
lrf = 0.0001
Momentum: 0.937
Weight Decay: 0.0005
Optimizer : AdamW
```

### 3. Training & Optimization

In this phase, training and optimization of the YOLO model are conducted. The training process involves presenting the Coral Life Forms Detection dataset to the YOLO architecture, where the model learns patterns and feature representations necessary for coral life forms detection system.

#### * Evaluasi Hasil Training

After the training process, the model is evaluated using a validation dataset to measure the accuracy of its predictions. Evaluation metrics used Precision, Recall, mAP50, mAP(50-95), providing a comprehensive overview of the model's performance in detection tasks. 

#### * Validation Results on Each Classes

**YOLOv8x :**
<img align="center" src= https://github.com/daniui/Machine-Learning-Project/blob/3a68096ff1f1050ba6a26c99dc459ede9d721033/CV%20Indonesia%20AI%20Bootcamp/Final%20Project/Assets/Screenshot%202024-02-13%20at%2011.40.04.png >
<img align="center" src= https://github.com/daniui/Machine-Learning-Project/blob/3a68096ff1f1050ba6a26c99dc459ede9d721033/CV%20Indonesia%20AI%20Bootcamp/Final%20Project/Assets/Screenshot%202024-02-13%20at%2012.02.15.png>
<img align="center" src= https://github.com/daniui/Machine-Learning-Project/blob/3a68096ff1f1050ba6a26c99dc459ede9d721033/CV%20Indonesia%20AI%20Bootcamp/Final%20Project/Assets/Screenshot%202024-02-13%20at%2012.02.30.png>

## ★ The Results

### Predict on Video

Here is the prediction result tested on a video of coral reef survey, please click the image to see the video results on YouTube:

[![Video Result](https://github.com/triwahyupra/project-coral-monitoring/blob/6bfd0463506ee3eecb6f7b5e107ce5bf7a68b7b0/assets-finalproject/inference.jpeg)](https://youtu.be/Rq34tTZci3A)


## Explore the Code!

The main notebook used for Model Development & Optimization can be accessed at the following link:
[YOLOv8x-Coral Detection](https://github.com/daniui/Machine-Learning-Project/blob/9953e58d6532daf36d32fec7a2279972f210f10a/CV%20Indonesia%20AI%20Bootcamp/Final%20Project/Hillmy_Rahmadani_Final_Project_Coral_Object_Detection_YOLOv8x.ipynb)

## 📧 Contact

If you have any questions, feedback, or would like to contribute to this project, feel free to contact the following:

- Nama: [ Hilmy Rahmadani ]
- Email: [ rahmadanihilmy@gmail.com ]
- LinkedIn: [ [Hilmy Rahmadani](https://www.linkedin.com/in/hilmyrahmadani/)
 
Thank you for your support and contributions!
