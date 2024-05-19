# ECG_signal_project
# MIT-BIH Arrhythmia Database Analysis and Classification

## Project Description
This project demonstrates the process of reading, processing, and classifying ECG signals from the MIT-BIH Arrhythmia Database. The goal is to extract QRS complexes, label them, and use a convolutional neural network (CNN) to classify the signals as either normal or abnormal.

## Requirements
To run this project, you need to install the following dependencies:
- Python 3.x
- WFDB library
- Matplotlib library
- NumPy library
- Pandas library
- Scikit-learn library
- tensorflow
- keras

You can install the required packages using the following command:
pip install wfdb matplotlib numpy pandas scikit-learn tensorflow keras

## Directory Setup
Ensure the MIT-BIH Arrhythmia Database is downloaded and the working directory is set to its location. Update the os.chdir path as necessary.

## Code Overview
### 1-Directory Setup and Record Listing
Set the working directory and list the contents of the MIT-BIH Arrhythmia Database.
Remove unnecessary files from the directory list.

### 2-Reading and Plotting Records
Read a specific record and its annotations.
Plot the record with annotations.

### 3-Beat and Label Extraction
Function extract_beats_and_labels extracts beats and their corresponding labels from the signals.
Loop through all records to extract beats and labels.

### 4-Data Preparation
Combine extracted beats and labels.
Save the combined data to a CSV file.

### 5-Data Filtering and Sampling
Filter and sample normal and abnormal beats.
Save the sampled data to a new CSV file.

### 6-Data Splitting and Label Encoding
Split the data into training and testing sets.
Encode the labels.

### 7-CNN Model Definition and Training
Define a CNN model for classifying the beats.
Compile and train the model using the training data.
Evaluate the model on the test data.

### 8-Model Evaluation
Calculate accuracy, precision, recall, F1-score, and confusion matrix.
Plot the ROC curve.
Plot a random signal from the test set and predict its label.

# link to download data
https://physionet.org/content/mitdb/1.0.0/

## Usage
Run the Script
Ensure the MIT-BIH Arrhythmia Database is in the specified directory.
Run the script to process the data, train the model, and evaluate its performance.

# Notes
-Ensure the working directory is set correctly to the location of the MIT-BIH Arrhythmia Database.
-Adjust the sampto parameter as needed to read more or fewer samples.
-The CNN model parameters (e.g., layer sizes, dropout rates) can be tuned to improve performance.
-Handle potential issues with imbalanced classes by using techniques such as oversampling, undersampling, or class weighting.

Feel free to reach out if you have any questions or need further assistance!
