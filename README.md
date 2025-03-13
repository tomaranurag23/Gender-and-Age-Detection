# Gender and Age Detection using OpenCV and Python

## Overview
This project implements **Gender and Age Detection** using OpenCV and a pre-trained deep learning model. It takes an input image or video stream, processes facial features, and predicts the gender and age of detected faces.

## Features
- Detects faces in images or real-time video streams.
- Predicts **gender** (Male/Female).
- Estimates **age** within predefined ranges.
- Uses a deep learning model for high accuracy.

## Requirements
Ensure you have the following dependencies installed before running the project:

```bash
pip install opencv-python numpy argparse
```

### Additional dependencies
- OpenCV
- NumPy
- Pre-trained Caffe model for face detection

## Pre-trained Models
The project utilizes the following models:
- **Face Detection Model:** `opencv_face_detector.caffemodel` (uses Caffe framework)
- **Age Detection Model:** `age_net.caffemodel`
- **Gender Detection Model:** `gender_net.caffemodel`

### Download Pre-trained Models
You can download the required models from OpenCV’s GitHub or other trusted sources and place them in the `models/` directory.

## Usage
### Running the script
Use the following command to run the detection script on an image:
```bash
python detect.py --image input.jpg
```

For real-time detection using a webcam:
```bash
python detect.py --video 0
```

## File Structure
```
│── models/                 # Pre-trained models
│── detect.py               # Main detection script
│── README.md               # Project documentation
│── requirements.txt        # List of dependencies
```

## Output Example
The script will output the processed image/video with predicted gender and age displayed over detected faces.

## License
This project is open-source and available under the **MIT License**.

## Acknowledgments
- OpenCV’s pre-trained models
- Deep learning frameworks for facial analysis

Feel free to contribute and enhance this project!

