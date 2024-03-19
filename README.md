# Face Anotation System

This repository contains a project for real-time face recognition using OpenCV and deep learning techniques. The system is capable of comparing faces from two images to determine if they belong to the same person, leveraging the power of Convolutional Neural Networks (CNN) for efficient and accurate face recognition.

## Table of Contents

- [Getting Started](#getting-started)
- [Prerequisites](#prerequisites)
- [Usage](#usage)
- [Approach](#approach)
- [Repository Files Navigation](#repository-files-navigation)
- [Contributing](#contributing)
- [License](#license)

## Getting Started

To get started with this project, follow these steps:

1. Clone the repository:
   ```
   git clone https://github.com/yourusername/Face-Recognition-System.git
   cd Face-Recognition-System
   ```
2. Create a dataset of face images and place them in the `dataset` folder.
3. Extract facial embeddings by running:
   ```
   python extract_embeddings.py
   ```
4. Train the SVM model:
   ```
   python train_model.py
   ```
5. Test the model:
   ```
   python recognize_video.py
   ```

## Prerequisites

- **OpenCV**: An open-source computer vision library used for image and video processing.
- **face_recognition**: A library for face recognition built using dlib's state-of-the-art face recognition built with deep learning.
- **NumPy**: A library for the Python programming language, adding support for large, multi-dimensional arrays and matrices, along with a large collection of high-level mathematical functions to operate on these arrays.

## Usage

To run the face recognition script, use:
```
python face_recognition.py
```

This script will load two images, detect faces in each, compute their face encodings, and compare these encodings to determine if the faces are the same.

## Approach

The project uses OpenCV for image processing and the face_recognition library for face detection and encoding. The approach involves:

- Loading two images.
- Converting the images to RGB format.
- Detecting faces within each image using face_recognition.
- Computing face encodings for each detected face.
- Comparing the face encodings to determine if the faces are the same.
- Displaying the comparison results and face distance.

## Repository Files Navigation

- `face_recognition.py`: The main script for running the face recognition system.
- `requirements.txt`: Lists the Python dependencies required for the project.
- `images`: Directory containing the images used for face recognition.
- `dataset`: Directory containing the dataset of face images.
- `extract_embeddings.py`: Script for extracting facial embeddings.
- `train_model.py`: Script for training the SVM model.
- `recognize_video.py`: Script for testing the model.

## Contributing

Contributions are welcome! Please feel free to submit a pull request or open an issue if you find any bugs or have suggestions for improvements.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
```

This README provides a comprehensive guide to setting up, using, and contributing to your face recognition project. It outlines the necessary steps for initial setup, details the project's dependencies, and explains how to use the system. Additionally, it offers a brief overview of the project's approach and navigates the repository's file structure.