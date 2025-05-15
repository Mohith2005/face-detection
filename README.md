Project Title:
Automated Face Recognition and Image Sorting System

Objective:
To develop an automated system that scans a collection of images, detects faces, and identifies matches with a predefined reference image. The system then extracts and stores all matching images into a dedicated output directory, enabling efficient facial identification and archival.

Project Description:
This project utilizes computer vision and deep learning-based face recognition to streamline the process of face matching across large image datasets. It leverages the face_recognition library powered by deep neural networks to encode facial features and compute similarity metrics. The workflow includes loading a reference face image, extracting its facial encoding, and scanning a target directory to find images containing faces that closely resemble the reference.

The matching operation is conducted by comparing facial encodings with a specified similarity threshold, and successfully matched images are copied to an output directory. The process is fully automated and generates a log file recording all matches and any processing errors.

Key Features:
Face Encoding: Generates a 128-d feature vector from the reference image using deep learning.

Face Detection and Matching: Scans each image for faces, encodes them, and compares against the reference encoding.

Customizable Threshold: Users can fine-tune the face match sensitivity via a configurable threshold.

Batch Processing: Efficiently handles large-scale datasets using tqdm for progress visualization.

Logging: Maintains a comprehensive log (match_log.txt) of matches and exceptions encountered during processing.

Output Management: Copies matched images into a structured output directory.

Technology Stack:
Language: Python 3.x

Libraries:

face_recognition (based on dlib)

OpenCV (cv2)

tqdm for progress tracking

os, glob, shutil for filesystem operations
