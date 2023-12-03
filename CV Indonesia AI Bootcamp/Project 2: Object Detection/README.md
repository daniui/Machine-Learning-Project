## Project 2: Object Detection, Person Tracking
## Our Team
1. Hilmy Rahmadani (me)
2. Hendra Ronaldi
3. Fitrah Ramadhan Reza
4. Harrison
5. I Putu Ananta Yogiswara
6. Fathurrahman Hernanda Khasan
7. Satriaji Najh Darmawan
8. Tri Wahyu Prabowo
9. Yurixa Skhinatul Putri
10. Nadya Novalina

## Project Overview
For our Second project we did a Person Tracking/Detection 

For this project we do a group research on 2 suggested model (Faster R-CNN and YOLO) with its variations:
1. Faster R-CNN with GoogleNet as Backbone ([Hilmy Rahmadani]() & [Hendra Ronaldi]())
2. [Faster R-CNN with MobileNet as Backbone]() (Fathurrahman Hernanda Khasan & Fitrah Ramadhan Reza)
3. Faster R-CNN with ResNet50 as Backbone ([Harrison]() & [I Putu Ananta Yogiswara]())
4. YOLO v3 ([Satriaji Najha Darmawan]() & [Tri Wahyu Prabowo]())
5. [YOLO v5] (Tri Wahyu Prabowo & Yurixa Sakhinatul Putri)
6. [YOLO v8]() (Satriaji Najha Darmawan & Nadya Novalina)
Notes : This repository will be focused on model that i worked on (Faster R-CNN with googlenet as backbone), and the team presentation result can be seen [here]()

## Dataset 
COCO-2017 from fiftyone was used in this project. it was sampled down to 4800 data (4000 train, 400 validation, 400 test). For this project we use person class only in detection.

## Experiment Result (Faster R-CNN with Googlenet as backbone)
we achieve mAP as follows
![image](https://github.com/daniui/Machine-Learning-Project/assets/120458194/da8cd558-d18c-447d-add1-c4d2946f1a4a)

and test/train loss as follows: 
-
Classification Report
-

PR Curve
-

Example Predictions:
![image](https://github.com/daniui/Machine-Learning-Project/assets/120458194/0a764cbd-23bb-41e4-ae7c-8b49a770ec0d)

## Dependencies
This project requires Python 3 and the following Python libraries installed:

Basic Libraries: NumPy, Matplotlib, Pandas

Deep-learning Frameworks: PytorchVision, FiftyOne

📨 That's all, for any discussion kindly contact me here: www.linkedin.com/in/hilmyrahmadani
