# ASL Fingerspelling Recognition
  
This project focuses on recognizing American Sign Language (ASL) fingerspelling using deep learning models. The goal is to accurately classify ASL gestures, leveraging a combination of CNNs and Transformer models. The project achieved a top 10% ranking on the Kaggle leaderboard.  
     
## Overview      
  
The ASL Fingerspelling Recognition system utilizes a two-part approach:
 
1. **CNN Model for Hand Landmark Detection**:
   - Developed a Convolutional Neural Network (CNN) using TensorFlow to classify ASL fingerspelling images.
   - Achieved 85% validation accuracy by leveraging Mediapipe for hand keypoint extraction.
  
2. **Transformer Model for Temporal Dependencies**:
   - Implemented a Transformer model to capture the temporal sequence of hand key points.
   - Utilized positional embeddings and self-attention to boost recognition accuracy.
   - Employed the Adam optimizer and dropout layers to mitigate overfitting.

## Dataset

The dataset is sourced from the [ASL Fingerspelling Kaggle Competition](https://www.kaggle.com/competitions/asl-fingerspelling), containing sequences of images representing fingerspelled letters.

- The dataset is processed using TFRecord files for efficient input handling.

## Acknowledgments

Mediapipe for hand keypoint detection.
TensorFlow Lite.
