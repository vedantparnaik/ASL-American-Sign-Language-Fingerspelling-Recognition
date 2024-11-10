# ASL Fingerspelling Recognition

This project focuses on recognizing American Sign Language (ASL) fingerspelling using deep learning models. The goal is to accurately classify ASL gestures, leveraging a combination of CNNs and Transformer models. The project achieved a top 10% ranking on the Kaggle leaderboard.

## Overview

The ASL Fingerspelling Recognition system utilizes a two-part approach:

1. **CNN Model for Hand Landmark Detection**:
   - Developed a Convolutional Neural Network (CNN) using TensorFlow and Keras for classifying ASL fingerspelling images.
   - Achieved 85% validation accuracy by leveraging Mediapipe for hand keypoint extraction.

2. **Transformer Model for Temporal Dependencies**:
   - Implemented a Transformer model to capture the temporal sequence of hand keypoints.
   - Utilized positional embeddings and self-attention to boost recognition accuracy.
   - Employed the Adam optimizer and dropout layers to mitigate overfitting.

## Dataset

The dataset is sourced from the [ASL Fingerspelling Kaggle Competition](https://www.kaggle.com/competitions/asl-fingerspelling), containing sequences of images representing fingerspelled letters.

- The dataset is processed using TFRecord files for efficient input handling.

## Installation

Clone the repository and install the required packages:

```bash
git clone <repository-url>
cd asl-fingerspelling-recognition
pip install -r requirements.txt


## Usage
The entire project is contained within the Jupyter notebook final-edit.ipynb.

Open the Notebook
Launch Jupyter and open final-edit.ipynb:

bash
Copy code
jupyter notebook final-edit.ipynb
Run the Cells
Execute the cells in the notebook sequentially. The notebook includes:

Data preprocessing using Mediapipe.
Training of the CNN model.
Training of the Transformer model.
Inference and evaluation.

## Results
Validation Accuracy (CNN Model): 85%
Test Accuracy (Combined Model): 74.3%
Ranked in the top 10% of the Kaggle competition.

## Model Export
The final trained model was converted to TensorFlow Lite for efficient inference. The notebook contains code for exporting the model as model.tflite.

## Files
final-edit.ipynb: The main notebook containing all code, including data preprocessing, model training, and evaluation.
model.tflite: The exported TensorFlow Lite model (generated from the notebook).

## Acknowledgments
Kaggle ASL Fingerspelling Competition: Link to Competition
Mediapipe for hand keypoint detection.

## License
This project is licensed under the MIT License - see the LICENSE file for details.
