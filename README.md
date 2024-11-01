# Face Attendance System

This project implements a face attendance system that tracks individuals by recognizing their faces in real-time. Using the **face_recognition** library, the system retrieves face encodings from a specified directory of images. When a face is detected in the video frame, the system displays the individual's name and logs their attendance in a CSV file if they are not already recorded.

# Features

- Real-time face detection and recognition
- Displays names of recognized individuals on the screen
- Automatically logs attendance to a CSV file
- Uses specified images for face encodings

# How It Works

1. **Face Encodings**: The system loads images from a specified directory. Each image should be named after the individual it represents. The face encodings are generated from these images.

2. **Real-Time Recognition**: The application captures video frames from a camera, checking for faces against the loaded encodings.

3. **Attendance Logging**: When a recognized face is detected, the corresponding name is displayed. If the individual's name is not already in the attendance log, the system adds it along with a timestamp to a CSV file.

# Requirements

To run this project, make sure you have the following libraries installed:

- `numpy`
- `opencv-python`
- `face_recognition`
- `pandas` (optional, for handling CSV files)
