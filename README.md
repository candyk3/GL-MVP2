# GL-MVP2
## Auto Object Detection
## Introduction
This Project utilizes Yolov9 Model for automatic object detection. The weights have been imported through Ultralytics and the images are inputed into the Model to generate Bounding boxes of each object that the model can detect. The generated bounding boxs are then used as a parameter to create Segmentation Masks for each individual object within a bounding Box. This can further be used to generate Polygons out of all the Masks that are generated, thus, reducing the time and the resources alloted to manually annotating each object in an image.

## Features
### YOLOv9 Model
This model demonstrates remarkable improvements in efficiency, accuracy, and adaptability, setting new benchmarks on the MS COCO dataset. This model is used to generate bounding boxes in the x1, y1, x2, y2 format where x1 and y1 are the coordinates of the top left corner of the bounding box and the x2 and y2 coordinates indicate the bottom right corner of the bounding box. 

Unfortunately, YOLOv9 may struggle with detecting and accurately identifying objects that are partially overlapping, which can be common in real-world scenarios.

## ![Screenshot 2024-07-14 221940](https://github.com/user-attachments/assets/317f993e-6f67-4ffb-8137-c2c0b4109b44)

### Segment Anything Model
SAM generates masks automatically, creates segmentation masks using bounding boxes, and converts object detection datasets into segmentation masks. Using the Bounding boxes as parameters, the model takes in the image using in setimage() in a numPy array format. The Model then uses each bounding box to predict and plot the segmentation mask of each object within the bounding boxes. 





