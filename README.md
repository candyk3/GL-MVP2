# GL-MVP2
## Auto Object Detection
## Introduction
This Project utilizes Yolov9 Model for automatic object detection. The weights have been imported through Ultralytics and the images are inputed into the Model to generate Bounding boxes of each object that the model can detect. The generated bounding boxs are then used as a parameter to create Segmentation Masks for each individual object within a bounding Box. This can further be used to generate Polygons out of all the Masks that are generated, thus, reducing the time and the resources alloted to manually annotating each object in an image.

## Features

