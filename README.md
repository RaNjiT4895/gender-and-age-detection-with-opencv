# gender-and-age-detection-with-opencv
# Real-Time Face Detection and Demographic Prediction

## Overview

This project implements a real-time face detection system that identifies human faces in images or video streams. It then predicts the gender and age group for each detected face using pre-trained deep learning models. The system provides a graphical representation by drawing bounding boxes around detected faces and overlaying the predicted gender and age on the image or video.

## Features
- Detect multiple faces in real-time from images or video streams.
- Predict gender (Male/Female) and age group for each detected face.
- Draw bounding boxes around detected faces and overlay demographic predictions.
- Configurable confidence threshold for face detection.

## Requirements
- Python 3.x
- OpenCV (`opencv-python` and `opencv-contrib-python`)
- Pre-trained models for face detection, age prediction, and gender prediction.

## Setup

### Install Dependencies

To run this project, you need to install the following dependencies:

- `opencv-python` for basic OpenCV functionality
- `opencv-contrib-python` for additional OpenCV features, including deep learning (DNN) support

### Installation

You can install the required dependencies by running the following command:

```bash
pip install opencv-python opencv-contrib-python
```

### Pre-trained Models

Download the following pre-trained models and save them in the project directory:

- **Face Detection Model:**
  - `opencv_face_detector.pbtxt`
  - `opencv_face_detector_uint8.pb`

- **Age Prediction Model:**
  - `age_deploy.prototxt`
  - `age_net.caffemodel`

- **Gender Prediction Model:**
  - `gender_deploy.prototxt`
  - `gender_net.caffemodel`

You can find these models on the OpenCV GitHub repository or other sources that provide pre-trained deep learning models for age and gender prediction.

## How It Works

- **Face Detection:** The system uses a pre-trained deep learning model (`opencv_face_detector`) to detect faces in the input image or video stream.
- **Gender Prediction:** For each detected face, the system uses the `gender_net` model to predict whether the person is male or female.
- **Age Prediction:** The system also predicts the age group of each detected face using the `age_net` model.
- **Visualization:** The system overlays bounding boxes on the faces with annotations showing the predicted gender and age.

## Contributing

If you would like to contribute to this project, feel free to fork the repository and submit a pull request. Contributions are welcome, and suggestions for improvement are appreciated.


## Acknowledgements

- OpenCV for face detection and DNN functionality.
- Pre-trained models for age and gender prediction.


