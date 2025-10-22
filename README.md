# GTZAN-Dataset-Music-Genre-Classification
A machine learning project to classify music genres from the GTZAN dataset using Python, Librosa, and Scikit-learn.

**🎵Music Genre Classification with GTZAN**
This project uses machine learning to classify music into 10 different genres based on audio features. It uses the well-known GTZAN dataset and leverages Python libraries like librosa for audio processing and scikit-learn for modeling.

📋 Table of Contents
Overview


**Overview**
The goal of this project is to build and evaluate a classifier that can accurately predict the genre of a 30-second audio clip. This notebook covers the complete machine learning workflow, from loading audio data to feature extraction, model training, and evaluation.

The 10 genres in the dataset are: blues classical country disco hiphop jazz metal pop reggae rock

✨ **Features**
**Audio Processing**: Uses librosa to load audio files and extract features.

**Feature Extraction**: Analyzes various audio characteristics, including:

Mel-Frequency Cepstral Coefficients (MFCCs)

Spectral Centroid

Spectral Rolloff

Chroma Features

Zero-Crossing Rate

**Data Visualization**: Plots waveforms and spectrograms using librosa.display and matplotlib.

**Machine Learning**: Implements and compares several classification models, such as:

K-Nearest Neighbors (KNN)

Support Vector Machine (SVM)

Random Forest

**Model Evaluation**: Assesses model performance using accuracy, classification reports, and confusion matrices.

💾**Dataset**
This project uses the GTZAN Genre Collection Dataset. Due to its size, the dataset itself is not included in this repository.

Source: You can download the dataset from or its .

Contents: The dataset consists of 1,000 audio files (30 seconds each), with 100 files for each of the 10 genres. A pre-computed feature CSV (features_30_sec.csv) is often used for faster analysis.

🚀 **Installation**
To run this project locally, follow these steps:

Clone the repository:

Install the required libraries:

If you don't have a requirements.txt file, you can manually install the main packages:

Download the Dataset:

Download the GTZAN dataset (e.g., features_30_sec.csv or the .wav files).

Place the data in a designated folder (e.g., a new /data folder).

Run the Notebook:

Launch Jupyter Notebook:

Open the .ipynb file and run the cells.

⚙️ **Project Pipeline**
Data Loading: The features_30_sec.csv file is loaded into a pandas DataFrame.

Playing The Audio: just like exploratory data analysis the a clip was played from the dataset

Visualizing Audio: The audio that played was also visualized in order to view its audio characteristics in visual form

Spectral roll-off

Zero-crossing Rate

Label Encoding: The text-based genre labels (e.g., 'blues') are converted into numeric form (e.g., 0) using LabelEncoder.

Feature Scaling: All numeric features are standardized using StandardScaler to ensure they have a mean of 0 and a standard deviation of 1. This is critical for models like SVM and KNN.

Train-Test Split: The dataset is split into training (67%) and testing (33%) sets.

Model Training & Evaluation: Several classifiers are trained on the training data and evaluated on the test data.

📈 **Results**
After training and testing, the models achieved the following performance:

The test loss is : 0.5563529133796692 
The test accuracy is : 0.900212287902832
