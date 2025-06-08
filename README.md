# AI-Powered ECG-Based Ischemia Detection Using Deep Learning

This project showcases the application of Artificial Intelligence in healthcare by developing a deep learning model to classify ECG signals for the detection of Ischemia. The model is built using PyTorch and is designed to distinguish between a normal sinus rhythm and one indicative of ischemia from 12-lead ECG recordings.

## Project Overview

The primary goal of this project is to build and train a robust deep learning model capable of accurately classifying ECG signals. This addresses a critical need for early and accurate cardiac diagnostic support, demonstrating the potential of AI in real-world healthcare applications.

### Key Features:

* **End-to-End ECG Analysis:** The project covers the complete workflow, from data acquisition and preprocessing to model training and evaluation.
* **Deep Learning Model:** A Fully Convolutional Network (FCN) is implemented in PyTorch, an architecture well-suited for time-series data like ECG signals.
* **High Accuracy:** The model achieves a high validation ROC AUC of 0.99, indicating excellent classification capability.

## Getting Started

To get started with this project, clone the repository and install the necessary dependencies.

### Prerequisites

You will need Python 3 and the following libraries. You can install them using pip:

```bash
pip install torch scipy numpy tqdm neurokit2 scikit-learn matplotlib plotly keras ecg_plot wfdb pandas opencv-python
Datasets

The ECG datasets for Normal Sinus Rhythm and Ischemia were obtained from Kaggle:

Ischemia Dataset: https://www.kaggle.com/datasets/bjoernjostein/ischemia-dataset
Normal Sinus Rhythm Dataset: https://www.kaggle.com/datasets/bjoernjostein/normalsinusdataset
You can use kagglehub to download the datasets as shown in the code.

Usage
The main script ischemia_classification.py handles the entire workflow, including data loading, preprocessing, model training, and evaluation.

To run the script, execute the following command in your terminal:

Bash
python ischemia_classification.py
The script will:

Download and preprocess the ECG data.
Build and train the FCN model.
Evaluate the model's performance and display the results.
Save the trained model as Ischemia_Classification.pth.
Ethical Considerations and Limitations
Clinical Decision Support: This model is intended to assist clinicians and should not be used as a replacement for professional medical advice. Clinical decisions should always be made by qualified medical professionals.
Data Privacy and Security: All patient data should be handled with strict confidentiality and in compliance with privacy regulations.
Dataset Limitations: The dataset used in this project may not be fully representative of the general population, which could limit the model's generalizability.
Acknowledgments
This project is based on and adapted from the "Median Heartbeat Classification - Ischemia" Kaggle notebook by Bjoern Jostein.

