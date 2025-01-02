# Speech Emotion Recognition

## Overview
This project uses machine learning techniques to implement a Speech Emotion Recognition (SER) system. The goal is to accurately classify the emotional state of a speaker based on audio input. The system utilizes features extracted from speech signals, primarily Mel-Frequency Cepstral Coefficients (MFCC), to train and evaluate various classification models.

## Table of Contents
- [Installation](#installation)
- [Dataset](#dataset)
- [Methodology](#methodology)
- [Result](#result)

## Installation
-  Clone the GitHub repository and install the required dependencies
   ```bash
   git clone https://github.com/yourusername/Speech_Emotion_Recognition.git
   cd Speech_Emotion_Recognition
   pip install -r requirements.txt
   ```
   - Run the main script to train and evaluate the models i.e. Composite_Classifier.ipynb

## Dataset
This project utilizes two primary datasets:
- RAVDESS: The Ryerson Audio-Visual Database of Emotional Speech and Song.
- TESS: Toronto Emotional Speech Set.

Both datasets include multiple emotional expressions recorded in controlled environments, which are critical for training our models effectively.

## Methodology
The methodology encompasses several steps including 
- Data preparation and feature extraction (MFCC, Chroma, Mel) using Librosa.
- Individual models SVM, KNN, and MLP are developed with hyperparameter tuning for each one of them was also performed along with normalization of the data.
- The Random Forest Classifier with ensemble method was used to create the final composite model with the predictions from the base models as input.

## Result
The project successfully achieved a model with high accuracy and robustness in emotion recognition from speech data. The composite model achieved the highest accuracy of 83.60% with an F1-Score (macro) of 0.8196 using only MFCC features.
