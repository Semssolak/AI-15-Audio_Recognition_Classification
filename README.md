# Sound Signal Classification Using Deep Learning
## Project Overview
This project consists of three main steps:

1. Dataset Preparation and Feature Extraction:
Extract sound signal features from audio files using Mel-Frequency Cepstral Coefficients (MFCC).

2. Model Building and Training:
Build a Convolutional Neural Network (CNN) model and train it with the prepared dataset.

3. Prediction:
Predict the class of an audio file using the trained model.

## Dataset
We will use the [UrbanSound8K Dataset](https://urbansounddataset.weebly.com/download-urbansound8k.html). Ensure that the dataset folder and the source code are in the same directory.

## Prerequisites
Install the required library using Anaconda Prompt:

```bash
conda install -c conda-forge librosa
```

## Step 1: Dataset Preparation and Feature Extraction
- **Objective:** Extract features from audio files using Mel-Frequency Cepstral Coefficients (MFCC).
- **Concept:** MFCCs are coefficients that collectively make up a Mel-frequency cepstrum, which represents the short-term power spectrum of a sound.

Process:
1.Load and preprocess audio files.
2.Extract MFCC features using the librosa library.
3.Store the features and labels in a dataframe.

## Step 2: Building and Training the CNN Model
- **Objective:** Build a CNN model and train it using the extracted features.

### Model Architecture:
1. Dense Layer: 125 units, ReLU activation, Dropout
2. Dense Layer: 250 units, ReLU activation, Dropout
3. Dense Layer: 125 units, ReLU activation, Dropout
4. Output Layer: Softmax activation

### Training:
- Compile the model with categorical crossentropy loss and the Adam optimizer.
- Train the model with the training dataset and validate it using the test dataset.
- 
## Step 3: Prediction
- **Objective:** Use the trained model to classify an audio file.
### Evaluation:
- Evaluate the model on the test dataset to determine its accuracy.

