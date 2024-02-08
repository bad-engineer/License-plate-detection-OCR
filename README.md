# License-plate-detection-OCR

In this project, we trained an object detection model to detect license plates and read characters on them. We also deployed the model on an OAK-D AI camera interfaced with a Jetson Nano for real-time object detection. 

# Dependencies

PyTorch >= 1.0.0\
opencv-python 3.x\
python 3.x\
Pillow\
NumPy\
scipy\
matplotlib

# Information About Trained Model
## Data Collection

We merged two license plate datasets from Roboflow for versatility:

https://universe.roboflow.com 
  
# Training and Testing

We trained the Yolov5 model on 120 epochs. The license plate is detected and cropped, the we use the Python EasyOCR library to extract characters from the cropped image. Finally, the string of characters is compared with a pre-defined list of 'authorized' number plates. This project demonstrates a system for automatic authorization of vehicles into secured areas.

# Results

![download (3)](https://github.com/bad-engineer/License-plate-detection-OCR/assets/147922795/f5d042d5-031e-4b09-bb46-546d8dca706a)
![download (4)](https://github.com/bad-engineer/License-plate-detection-OCR/assets/147922795/0564f14a-8da6-4b23-a338-2eecbc5e620a)

![download](https://github.com/bad-engineer/License-plate-detection-OCR/assets/147922795/587cf9da-632e-406f-bb50-1a58b7b2e8fc)
![test_image1](https://github.com/bad-engineer/License-plate-detection-OCR/assets/147922795/46e4738b-62a5-4849-ae08-cade297d73f2)
