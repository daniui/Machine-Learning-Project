# Project 1 Face Recognition
First group project in Indonesia AI computer vision bootcamp
## Our Team
1. Hilmy Rahmadani (me)
2. Hendra Ronaldi
3. Fitrah Ramadhan Reza
4. Harrison
5. I Putu Ananta Yogiswara
6. Fathurrahman Hernanda Khasan
## Project Overview
For our fisrt project we did a face recognition for gender classification that is useful for a lot industry, from retail and healthcare to banking and entertainment, various industries are harnessing the capabilities of facial recognition to streamline processes, enhance security and offer personalized experiences.
For this project we do a group research on 3 suggested model:
1. [Googlenet](https://github.com/daniui/Machine-Learning-Project/blob/1665282e96cd8552c035666f5b4f3673c0393c3a/CV%20Indonesia%20AI%20Bootcamp/Dani_CVB_project_1_Face_Recognition_googlenet.ipynb). (Hilmy Rahmadani & I Putu Ananta Yogiswara)
2. [VGG](https://github.com/daniui/Machine-Learning-Project/blob/1665282e96cd8552c035666f5b4f3673c0393c3a/CV%20Indonesia%20AI%20Bootcamp/VGG.ipynb). (Hendra Ronaldi & Fathurrahman Hernanda Khasan)
3. [Resnet](https://github.com/daniui/Machine-Learning-Project/blob/1665282e96cd8552c035666f5b4f3673c0393c3a/CV%20Indonesia%20AI%20Bootcamp/Resnet.ipynb). (Harrison & Fitrah Ramadhan Reza)
Notes : This repository will be focused on model that i worked on (googlenet)
## Dataset 
Dataset [CelebA](https://mmlab.ie.cuhk.edu.hk/projects/CelebA.html) used in this project. It was sampled down and provided by the bootcamp to be consists of 5000 face images. The attribute information of the images can be seen [here](https://www.kaggle.com/datasets/jessicali9530/celeba-dataset/?select=list_attr_celeba.csv), we use the column Male as target for this project (-1 as Female and 1 as Male)
## Experiment Result (Googlenet)
For google net we achieve test/train accuracy as follows:
![image](https://github.com/daniui/Machine-Learning-Project/assets/120458194/e927578b-7112-41fe-9dca-ff10b7418ddd)

and test/train loss as follows: 
![image](https://github.com/daniui/Machine-Learning-Project/assets/120458194/62924f93-aabe-4598-b6f5-9977fc81d93d)

Confusion matrix:
![image](https://github.com/daniui/Machine-Learning-Project/assets/120458194/30fc15a5-bd81-4316-8490-364e1f4c9605)

Example Predictions:
![image](https://github.com/daniui/Machine-Learning-Project/assets/120458194/741c792f-609f-4212-a670-443fd4c0c8ac)

Recommendations : as we can see there is 1 false predictions, this raise suspiction that the model is not trained enough in recognizing female with a short hair. Therefore we need a lot more female data with short hair.

## Dependencies
This project requires Python 3 and the following Python libraries installed:

Basic Libraries: NumPy, Matplotlib, Pandas
Deep-learning Frameworks: Pytorch

📨 That's all, for any discussion kindly contact me here: www.linkedin.com/in/hilmyrahmadani
