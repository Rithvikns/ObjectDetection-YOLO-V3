## yolo_detection_images.py

The code in yolo_detection_images.py performs object detection on images using the YOLOv3 deep learning model with OpenCV's DNN module. It loads the YOLO model, COCO class labels, and processes images from the dev folder. Each image is resized and converted into a format suitable for YOLO, which then predicts object locations and class probabilities. Bounding boxes are filtered based on a confidence threshold (0.5), and Non-Maximum Suppression (NMS) is applied to remove overlapping detections. Each detected object is assigned a unique color, and a bounding box with a confidence score is drawn on the image.

If a person is detected, the modified image is saved to the dev1 folder. The script then displays the image for 500 milliseconds before processing the next one. This pipeline is useful for real-time object detection and can be extended for applications like security surveillance, autonomous vehicles, or crowd monitoring.


## yolo_detection_images4.py

This code performs license plate detection using a custom-trained YOLO model. It first enhances the sharpness of images from the test_out folder using PIL and saves them in test_out1. Then, it loads a YOLO model with a configuration file (obj.cfg), pre-trained weights (obj_60000.weights), and class labels from obj3.names. Each image is processed by resizing it, converting it into a YOLO-compatible format, and passing it through the model. The detected objects are filtered based on a confidence threshold (0.5), and Non-Maximum Suppression (NMS) removes overlapping bounding boxes.

If an object labeled "LP" (License Plate) is detected, the license plate region is cropped and saved in the LP folder. The script also draws bounding boxes around detections and displays the cropped license plate for 500 milliseconds. This pipeline is useful for automatic license plate recognition (ALPR) systems, which can be used in traffic monitoring, parking management, and law enforcement applications.

## yolo_detection_images6.py

This code performs triple-rider detection using the YOLOv3 object detection model. It first scans the tripleride folder, counts the number of images, and removes any corrupted files using PIL. Then, it loads the YOLO model with COCO class labels and processes each image by converting it into a format suitable for YOLO. The model detects objects in the image, filtering them based on a confidence threshold (0.0) and applying Non-Maximum Suppression (NMS) to remove overlapping bounding boxes.

For each processed image, the detected object labels are stored in a list. If the label "person" appears exactly three times (indicating a triple rider on a motorcycle), the image is saved in the test_out folder. The script also displays each image for 500 milliseconds before moving to the next one. This pipeline is useful for traffic law enforcement, particularly for detecting illegal triple-riding on motorcycles in real-time surveillance systems.


## yolo_detection_webcam.py

This code performs real-time object detection on a video using the YOLOv3 model. It loads a pre-trained YOLO model with COCO class labels and processes each frame of the video (om116.mp4). The model detects objects in each frame by resizing and converting the image into a YOLO-compatible format. The detected objects are filtered based on a confidence threshold (0.0), and Non-Maximum Suppression (NMS) is applied to remove redundant bounding boxes.

The script specifically looks for motorbikes and people, drawing bounding boxes around them and displaying confidence scores. Each processed frame is shown in a real-time window, and the detection results are printed in the console. The video feed continues until the user presses 'q' to exit. This approach is useful for traffic surveillance, accident detection, and law enforcement applications, enabling real-time monitoring of motorcycles and riders.


## yolo_detection_webcam1.py

This code performs motorbike detection in a video using YOLOv3. It loads a pre-trained YOLO model with COCO class labels and processes each frame from the input video (om1.mp4). The model detects objects by converting each frame into a YOLO-compatible format, filtering objects based on a confidence threshold (0.5), and applying Non-Maximum Suppression (NMS) to remove redundant detections.

If a motorbike is detected, the relevant region of the frame is extracted and saved as an image in the dev folder. The script runs in a loop, continuously processing and displaying each frame in real-time. It stops when the user presses 'q'. This setup is useful for traffic surveillance, vehicle tracking, and road safety monitoring by identifying and capturing images of motorbikes from live or recorded footage.

## yolo_detection_webcam2.py

This script uses YOLOv3 to detect motorbikes in a video (om116.mp4). It loads the pre-trained YOLO model with COCO dataset labels and processes each frame to identify objects. The model applies a confidence threshold of 0.0, ensuring all detections are considered before filtering them using Non-Maximum Suppression (NMS) with a threshold of 0.6 to remove overlapping bounding boxes.

If a motorbike is detected, the script crops the detected region and saves it in the tripleride folder. The processed frames are displayed in real-time, and the loop continues until the user presses 'q'. This implementation is useful for traffic monitoring, vehicle detection, and road safety analysis, capturing images of motorbikes for further inspection or dataset collection.



The weights file are hosted in the google drive , you can download using this link https://drive.google.com/drive/folders/1P0UAdttdqpdIWfhxXByRLKtQURNaky1H?usp=sharing
