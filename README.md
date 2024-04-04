
# Hand Sign Recognition Project

This project aims to recognize hand signs using machine learning. It consists of several Python scripts that collect hand images, extract hand landmarks, train a model, and make predictions.

## Project Overview

1. **Data Collection (`jjkD2.py`):**
   - Collects images of different hand signs using a webcam.
   - Stores the images in separate directories for each hand sign class.

2. **Hand Landmark Extraction (`jjkD3.py`):**
   - Processes the collected images.
   - Extracts hand landmarks using the MediaPipe library.
   - Normalizes the hand landmarks.
   - Saves the hand landmarks in a pickle file (`data.pickle`).

3. **Model Training (`jjkD4.py`):**
   - Loads the hand landmark data from `data.pickle`.
   - Splits the data into training and testing sets.
   - Trains a RandomForestClassifier model on the training set.
   - Evaluates the model's accuracy on the testing set.
   - Saves the trained model in a pickle file (`model.p`).

4. **Real-time Prediction (`jjkD5.py`):**
   - Uses the trained model to predict hand signs in real-time.
   - Captures hand landmarks from a webcam feed.
   - Maps the predicted class to the corresponding hand sign label.
   - Displays the predicted hand sign on the video feed.

## Usage

1. Run `jjkD2.py` to collect hand images.
2. Run `jjkD3.py` to extract hand landmarks and save them in `data.pickle`.
3. Run `jjkD4.py` to train the model and save it in `model.p`.
4. Finally, run `jjkD5.py` for real-time hand sign recognition.

## Requirements

- Python 3.x
- OpenCV
- MediaPipe
- scikit-learn


