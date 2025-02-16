## yolo_detection_images.py

The code in yolo_detection_images.py performs object detection on images using the YOLOv3 deep learning model with OpenCV's DNN module. It loads the YOLO model, COCO class labels, and processes images from the dev folder. Each image is resized and converted into a format suitable for YOLO, which then predicts object locations and class probabilities. Bounding boxes are filtered based on a confidence threshold (0.5), and Non-Maximum Suppression (NMS) is applied to remove overlapping detections. Each detected object is assigned a unique color, and a bounding box with a confidence score is drawn on the image.

If a person is detected, the modified image is saved to the dev1 folder. The script then displays the image for 500 milliseconds before processing the next one. This pipeline is useful for real-time object detection and can be extended for applications like security surveillance, autonomous vehicles, or crowd monitoring.
























The weights file are hosted in the google drive , you can download using this link https://drive.google.com/drive/folders/1P0UAdttdqpdIWfhxXByRLKtQURNaky1H?usp=sharing
