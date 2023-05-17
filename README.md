# Face Recognition Video Application

This repository contains a face recognition video application implemented using Python and OpenCV. The application detects and recognizes faces in recorded videos, displaying the recognized faces with their corresponding names in real-time.

## Features
- **Face Detection**: The application utilizes the Haar cascade classifier to detect faces in each frame of the recorded video. It uses a pre-trained model to identify facial features and locate faces accurately.
- **Face Recognition**: Once a face is detected, the application extracts the face region of interest (ROI) and resizes it to a standard size. It then uses the face_recognition library, which implements the deep learning-based face recognition algorithm, to encode the face and compare it with a set of known faces.
- **Known Faces**: The application loads a set of known faces and their corresponding encodings from CSV files. Each CSV file contains the encoding for a specific face along with the person's name. The application compares the face encoding of the detected face with the known faces to determine the closest match.
- **Real-time Display**: The application draws a rectangle around each detected face and displays the predicted label (name) for each recognized face in real-time. If the detected face matches a known face, the corresponding name is shown; otherwise, it displays "Unknown".
- **User-friendly Interface**: The application includes a user-friendly interface implemented using the tkinter library. It provides a file dialog window to select the recorded video file for processing.

## Requirements
- Python 3.x
- OpenCV
- face_recognition
- tkinter

## Usage
1. Install the required dependencies by running the following command:
pip install -r requirements.txt
2. Place the recorded video file you want to process in the same directory as the script.
3. Run the application by executing the following command:
python face_recognition_app.py
4. The application will open a file dialog window. Select the recorded video file you want to process.
5. The video will start playing, and the application will detect and recognize faces in real-time, displaying the recognized faces with their corresponding names.
6. To exit the application, press the 'q' key.

## Contributing
Contributions are welcome! If you have any ideas, suggestions, or improvements, please open an issue or submit a pull request.

