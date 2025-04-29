# Speech Emotion Recognition Using Deep Learning

## Project Overview

This project focuses on classifying emotions from speech recordings using Deep Learning techniques.  
The model architecture is built around the MobileNetV2 model, along with custom layers, applied to spectrogram-based pseudo-RGB images.

The project demonstrates how transfer learning significantly improves performance with a dataset like RAVDESS.

---

## Dataset

- **Name:** RAVDESS Emotional Speech Audio
- **Link:** [RAVDESS Dataset](https://www.kaggle.com/datasets/uwrfkaggler/ravdess-emotional-speech-audio)
- **Description:**  
  - 1,440 audio recordings (wav format)
  - 8 emotions: Neutral, Calm, Happy, Sad, Angry, Fearful, Disgust, Surprised
  - Balanced class distribution

---

## Approach

1. **Exploratory Data Analysis (EDA)**
   - Visualized emotion distribution
   - Inspected waveforms and spectrograms

2. **Feature Engineering**
   - Extracted Mel Spectrogram and MFCC features
   - Created 3-channel pseudo-RGB spectrogram images
   - Applied data augmentation (noise addition, pitch shift, time stretch)

3. **Models Implemented**
   - **Baseline:** CNN + BiLSTM model
   - **Advanced:** MobileNetV2 Transfer Learning (frozen base model + custom classification head)

4. **Optimization Techniques**
   - EarlyStopping
   - Learning Rate Reduction on Plateau
   - Data normalization for transfer learning

---

## Setup Instructions

1. Clone the repository:

```
git clone https://github.com/AndroGermisa2938/intro-to-deep-learning-final
cd speech-emotion-recognition
```

2. Download the data, and extract it under speech-emotion-recognition/data

3. Run the requirements.txt

```
pip install -r requirements.txt
```
