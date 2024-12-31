Real-Time Face Detection and Recognition Model

Overview

This project focuses on building a real-time face detection and recognition system using Haar feature-based cascade classifiers and a KNN (K-Nearest Neighbors) classifier. The system efficiently detects faces in live video streams and recognizes them with high accuracy under well-lit conditions, making it suitable for applications such as security systems, user authentication, and interactive systems.

Key Features

Real-Time Face Detection: Detects faces in live video feeds using Haar Cascade Classifiers.
Face Recognition with KNN: Recognizes detected faces using a KNN classifier (K = 3), enhancing recognition robustness.
High Accuracy: Achieves 95% detection accuracy in well-lit environments.
Real-Time Processing: Processes video frames at up to 30 FPS using OpenCV.
Scalable: Handles multiple face detections simultaneously in dynamic conditions.
Technologies Used

Programming Language: Python
Libraries:
OpenCV: For video frame processing and face detection.
NumPy: For numerical computations and data handling.
Logging: For tracking system performance and detections.
Installation
Clone the repository:

bash
Copy code
git clone https://github.com/Akashhverma/Real-time-face-detection.git  
cd Real-time-face-detection  
Install dependencies:
Ensure you have Python 3.7+ and install the required libraries:

bash
Copy code
pip install opencv-python opencv-python-headless numpy  
Download the Haar Cascade XML file:
Download the haarcascade_frontalface_default.xml file from the OpenCV GitHub repository and place it in the project directory.

Usage
Run the script:

bash
Copy code
python face_detection_knn.py  
Press 'q' to quit the application while it's running.

Code Overview
Haar Cascade Classifier: Used for detecting faces in grayscale frames.
KNN Classifier: A simple but effective algorithm trained on pre-labeled face data for recognition.
Logging: Keeps track of the number of faces detected and logs events to a file (webcam.log).
Sample Output
The system draws rectangles around detected faces and logs the detection events with timestamps.


Project Files
face_detection_knn.py: Main script for face detection and recognition.
haarcascade_frontalface_default.xml: Pre-trained Haar Cascade model for face detection.
webcam.log: Log file tracking detection events.
Future Enhancements
Support for low-light detection using adaptive histogram equalization.
Addition of face tracking using Kalman Filters.
Training the KNN classifier on a larger and more diverse dataset for improved recognition accuracy.

Integration with Streamlit or Flask for web-based deployment.

Contributors
Akash Verma
