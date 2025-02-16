# TRAFFIC RULES VIOLATION RECOGNITION FOR TWO WHEELER USING YOLO ALGORITHM


## INTRODUCTION

Bike is an extremely mainstream method of transportation in India. However, there is a high risk involved due to lack of protection.
 To decrease the involved risk, it is highly desirable for motorcycle riders to use helmet. That’s why the government has made it a punishable offense to ride a bike without helmet. 
The drawback of the current method where human intervention is required can be solved by our proposed method. 
Nowadays eveyone is moving towards automation and many countries have implemented automatic traffic surveillance sytem.
Here we are developing a system in which we are using a more efficient way which helps us in getting better results.

## OBJECTIVE

The main objective of the project work is to develop a system for
Detection of persons on the motorbikes who are not wearing the helmet  and triple riding while crossing the signals and junctions .
Sending an SMS to the concerned authority about the vehicle details of the person who violates the above-mentioned rule.
To improvise the metric(accuracy,speed and efficiency) to yield better results

## BLOCK DIAGRAM

![image](https://github.com/user-attachments/assets/bef31b2a-aaaa-4d26-9798-f7ee275f0b14)

## Flow Diagram

![image](https://github.com/user-attachments/assets/1906ded9-78a2-4e31-96d2-9b63212f5ffe)

## Methodology

STEP1 - A real time input video is fed to the model.
STEP2 - The model is previously trained with a dataset. Then the real time input is compared with dataset.
STEP3 - If the two-wheeler is detected in the input the process continues else the image is discarded.
STEP4 - After two-wheeler is detected, the pretrained model detects the rider wearing helmet and triple riding. If the rules are violated it goes to the next step else the image is discarded.
STEP5 - When the rules are violated an SMS alert will be sent to the concerned authority.  


