# SVM Face Detection - README

## Overview
This repository contains a Jupyter Notebook implementation of a face detection system using Support Vector Machines (SVM) with OpenCV's Haar Cascade classifier. The system can detect faces in images and predict whether they match a trained face dataset.

## Features
- **Face Detection**: Uses OpenCV's pre-trained Haar Cascade classifier for face detection
- **Feature Extraction**: Converts detected faces to grayscale and resizes them for processing
- **SVM Model**: Implements One-Class SVM for face recognition
- **Image Processing**: Includes preprocessing steps like grayscale conversion and resizing
- **Prediction**: Demonstrates how to make predictions on new face images

## Requirements
- Python 3.x
- OpenCV (`pip install opencv-python`)
- scikit-learn
- numpy
- matplotlib
- Jupyter Notebook (optional)

## Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/svm-face-detection.git
   ```
2. Navigate to the project directory:
   ```bash
   cd svm-face-detection
   ```
3. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

## Usage
1. Prepare your face dataset:
   - Place training images in the specified folder (`C:\\Users\\FC\\Desktop\\Face Detection` by default)
   - Name files in the format `[label]_[number].jpg` (e.g., `TonyStark_1.jpeg`)

2. Run the Jupyter Notebook:
   ```bash
   jupyter notebook SVM Face-Detection.ipynb
   ```

3. The notebook will:
   - Load and preprocess the face images
   - Train the One-Class SVM model
   - Demonstrate face detection and prediction on a test image

## File Structure
- `haarcascade_frontalface_default.xml`: OpenCV's Haar Cascade classifier for face detection
- `SVM Face-Detection.ipynb`: Jupyter Notebook containing the implementation
- Test images should be placed in the specified directory (modifiable in the notebook)

## Notes
- The current implementation uses a simple One-Class SVM approach
- For better accuracy, consider using more sophisticated face recognition techniques
- The path to the training images needs to be adjusted based on your system

## License
This project is licensed under the MIT License. 

## Contributing
Contributions are welcome! Please open an issue or submit a pull request for any improvements.
