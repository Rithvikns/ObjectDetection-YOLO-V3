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


## GUI

![image](https://github.com/user-attachments/assets/4a1bef2b-d215-4709-993d-efc58d40e5f4)

A GUI (graphical user interface) is a system of interactive visual components for computer software. 
A GUI displays objects that convey information, and represent actions that can be taken by the user.
Tkinter -It is the standard GUI library for Python. Python when combined with Tkinter provides a fast and easy way to create GUI applications.
  Hence we use Tkinter in our project For user interface for different applications.
We create buttons in the GUI page for each applications.

## YOLO V3 Network Architecture

![image](https://github.com/user-attachments/assets/73920392-4581-4b49-9130-47e540c10824)

YOLO v3 makes prediction at three scales, which are precisely given by downsampling the dimensions of the input image by 32, 16 and 8 respectively.
The first detection is made by the 82nd layer. For the first 81 layers, the image is down sampled by the network, such that the 81st layer has a stride of 32.

 If we have an image of 416 x 416, the resultant feature map would be of size 13 x 13. One detection is made here using the 1 x 1 detection kernel, giving us a detection feature map of 13 x 13 x 255.

Then, the feature map from layer 79 is subjected to a few convolutional layers before being up sampled by 2x to dimensions of 26 x 26. 

This feature map is then depth concatenated with the feature map from layer 61. 

Then the combined feature maps is again subjected a few 1 x 1 convolutional layers to fuse the features from the earlier layer (61). Then, the second detection is made by the 94th layer, yielding a detection feature map of 26 x 26 x 255.

## Output

![image](https://github.com/user-attachments/assets/79ae5518-0e44-4041-95b7-c810182ed849)

![image](https://github.com/user-attachments/assets/9fe95e23-799c-473c-b4ca-c51889bfbe10)

![image](https://github.com/user-attachments/assets/c1d06692-9e87-4771-bf21-4e492015f3bf)

![image](https://github.com/user-attachments/assets/1ae6b12d-785d-482d-9928-7df2d3efbb6f)

![image](https://github.com/user-attachments/assets/a7922aa4-f97d-4471-b45a-773edc803e68)

## Conclusion

As when compared to other algorithm YOLO is found be more advantageous and has higher efficiency and accuracy. Hence, we use the same approach to identify triple riding.
Since we are implementing our project using YOLO algorithm which is a CNN based approach, results are obtained at fastest speed ![image](https://github.com/user-attachments/assets/e2e8c99a-67f6-42a1-8c5e-a91468aeaf8b)

