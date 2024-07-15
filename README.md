# Motorcycle License Plate Extraction When Rider Isn't Wearing a Helmet

This project focuses on extracting motorcycle license plates if the rider or passenger is not wearing a helmet.

## Project Overview

### Workflow
1. **Object Detection:**
   - YOLOv5 algorithm is used to detect motorcycle riders, license plates, and riders' heads in images or video frames.

2. **Helmet Classification:**
   - ResNet50 image classifier determines whether the detected rider is wearing a helmet or not.

3. **Action on Non-Helmet Detection:**
   - If a helmet is not detected, the project saves the license plate number and captures the rider's image in separate folders.

### Example
![Example GIF](./bike_gif.gif)

## Download Models and Necessary Files
To run the code, download the following files and place them in your main project folder:

- **YOLOv5 Weight Files:**
  - [Small Version](https://drive.google.com/file/d/1LbX-YRBTgJZEIqQqmCpNq4CNQzoiA8p5/view?usp=sharing)
  - [Medium Version](https://drive.google.com/file/d/16ZDjUcX7vXQYPJ557dooN0em4mJmbJt7/view?usp=sharing)

- **Classification Model (ResNet50):**
  - [Download Link](https://drive.google.com/file/d/1OuOpgq99E5VKPtwUuFZ0GGety3YWjIQn/view?usp=sharing)

## Installation and Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/manikumarpula/Helmet-License_Plate_Detection.git
2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
3. Download and Place Model Files
    1. Download Model Files:
        Download YOLOv5 and ResNet50 model weights from the links above.
    2. Place Model Files:
        Place the downloaded model weights in the models/ directory of the project.
4. Output:
    1. Detected license plate numbers will be saved in the output/license_plates/ folder.
    2. Images of riders without helmets will be saved in the output/rider_images/ folder.
5. Requirements
    Python 3.x
    Torch (PyTorch)
    OpenCV
    NumPy
    PIL (Python Imaging Library)

