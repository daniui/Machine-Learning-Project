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
1. Faster R-CNN with GoogleNet as Backbone ([Hilmy Rahmadani](https://github.com/daniui/Machine-Learning-Project/blob/94d0f1ad1c3131526514168b131863330f270e40/CV%20Indonesia%20AI%20Bootcamp/Project%202%3A%20Object%20Detection/Dani_project%202_person%20tracking_Faster%20RCNN_googlenet.ipynb) & [Hendra Ronaldi](https://github.com/daniui/Machine-Learning-Project/blob/94d0f1ad1c3131526514168b131863330f270e40/CV%20Indonesia%20AI%20Bootcamp/Project%202%3A%20Object%20Detection/Hendra_Project_2_Person_Tracking_(Faster_R_CNN_GoogLeNet).ipynb
))
2. [Faster R-CNN with MobileNet as Backbone](https://github.com/daniui/Machine-Learning-Project/blob/94d0f1ad1c3131526514168b131863330f270e40/CV%20Indonesia%20AI%20Bootcamp/Project%202%3A%20Object%20Detection/fathurrahman_Mobile_net.ipynb
) (Fathurrahman Hernanda Khasan & Fitrah Ramadhan Reza)
3. Faster R-CNN with ResNet50 as Backbone ([Harrison](https://github.com/daniui/Machine-Learning-Project/blob/94d0f1ad1c3131526514168b131863330f270e40/CV%20Indonesia%20AI%20Bootcamp/Project%202%3A%20Object%20Detection/Harrison_fasterrcnn_rasnet50.ipynb) & [I Putu Ananta Yogiswara](https://github.com/daniui/Machine-Learning-Project/blob/94d0f1ad1c3131526514168b131863330f270e40/CV%20Indonesia%20AI%20Bootcamp/Project%202%3A%20Object%20Detection/putu_ananta_fasterrcnn_resnet50.ipynb))
4. YOLO v3 ([Satriaji Najha Darmawan](https://github.com/daniui/Machine-Learning-Project/blob/94d0f1ad1c3131526514168b131863330f270e40/CV%20Indonesia%20AI%20Bootcamp/Project%202%3A%20Object%20Detection/Satriaji_PersonDetection_trainingYOLOv3.ipynb) & [Tri Wahyu Prabowo]())
5. [YOLO v5](https://github.com/daniui/Machine-Learning-Project/blob/94d0f1ad1c3131526514168b131863330f270e40/CV%20Indonesia%20AI%20Bootcamp/Project%202%3A%20Object%20Detection/triwahyu_yolov5_yolov3_coco_persontracking.ipynb) (Tri Wahyu Prabowo & Yurixa Sakhinatul Putri)
6. YOLO v8 ([Satriaji Najha Darmawan](https://github.com/daniui/Machine-Learning-Project/blob/94d0f1ad1c3131526514168b131863330f270e40/CV%20Indonesia%20AI%20Bootcamp/Project%202%3A%20Object%20Detection/Satriaji_PersonDetection_trainingYOLOv8.ipynb) & [Nadya Novalina](https://github.com/daniui/Machine-Learning-Project/blob/94d0f1ad1c3131526514168b131863330f270e40/CV%20Indonesia%20AI%20Bootcamp/Project%202%3A%20Object%20Detection/Nadya_Project_2_yolov8m.ipynb))


Notes : This repository will be focused on model that i worked on (Faster R-CNN with googlenet as backbone), and the team presentation result can be seen [here](https://github.com/daniui/Machine-Learning-Project/blob/4eb648a18f55dfb8c62f6863a702c06bd8bea9d0/CV%20Indonesia%20AI%20Bootcamp/Project%202%3A%20Object%20Detection/Project%202.pdf)

## Dataset 
COCO-2017 from fiftyone was used in this project. it was sampled down to 4800 data (4000 train, 400 validation, 400 test). For this project we use person class only in detection.

## Experiment Result (Faster R-CNN with Googlenet as backbone)
we achieve mAP as follows
-

and test/train loss as follows: 
-
Classification Report
-

PR Curve
-

Example Predictions:
![image](https://github.com/daniui/Machine-Learning-Project/assets/120458194/da8cd558-d18c-447d-add1-c4d2946f1a4a)

## Dependencies
This project requires Python 3 and the following Python libraries installed:

Basic Libraries: NumPy, Matplotlib, Pandas

Deep-learning Frameworks: PytorchVision, FiftyOne

📨 That's all, for any discussion kindly contact me here: www.linkedin.com/in/hilmyrahmadani
