
# Title of Project

## Safety Helmet Detection Project using YOLOv5


# Introduction
This project uses YOLOv5, a real-time object detection system, to detect if a person is wearing a safety helmet in an image or video. The project is built using the PyTorch framework and is trained on a dataset of images containing people wearing seftey helmets and not wearing saftey helmets.


## Problem understanding
The use of safety helmets is crucial in various high-risk industries such as construction, mining, and manufacturing, to protect workers from head injuries in the event of an accident. Despite being mandatory in many countries, compliance with safety helmet regulations remains a challenge.

By using computer vision and machine learning algorithms, safety helmet detection systems can accurately monitor compliance in real-time, ensuring that workers are protected at all times. These systems can be integrated into existing security systems, such as security cameras, and can provide valuable insights into the safety culture of an organization.
## Data 
This dataset, contains 5000 images with bounding box annotations in the PASCAL VOC format for these 3 classes:

- Helmet;
- Person;
- Head.

The data set is downloaded from kaggle.


To downlad the data set you can refer to this link:-


https://www.kaggle.com/datasets/andrewmvd/hard-hat-detection

## Prerequisites
The following packages and libraries are required to run this project:

- Python 3.x
- Pandas
- NumPy
- Sklearn
- Matplotlib
- PyTorch
- OpenCV


## Task Done

- Problem Undertsatnding and Data Collection part are already Done 

### 1) Data Prepration
- Yolo requires the data into certain format (label,x_centre,y_centre, width, height). But here the format (x_min,y_min,x_max,img_height,img_width) is different than yolo's format.

- So first of all we convert the given format into required format

### 2) Train Yolo V5 on custom data set
- After preparing the data we passed it to yolo archhitecture and train the yolo v5 model on this data set
- After training we find the custom weights

### 3) Detection
- After find the best wieghts we try to detect the object from the avialble image 
- We have also prepared live detection file using opencv to detect saftey helmet in real time.Here we have passed our custom weights.





## Conclusion

The safety helmet detection project using YOLOv5 demonstrates the potential of deep learning in object detection and its applications in solving real-world problems. This project can be further improved by fine-tuning the model on a larger and more diverse dataset


