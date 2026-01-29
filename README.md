# Deepfake Detection CNN Model

A simple Convolutional Neural Network (CNN) baseline for classifying images as **Real (0)** or **Fake (1)** using TensorFlow/Keras and OpenCV. This project loads images from `real/` and `fake/` folders, trains a CNN, and evaluates performance on a held-out test set.

---

## Project Overview

**Goal:** Detect deepfake (synthetic) images using supervised binary classification.

**Approach:**
- Load and preprocess images with OpenCV (resize, RGB conversion, normalization)
- Build a CNN in Keras (Conv2D + MaxPooling + Dense + Dropout)
- Train with a train/validation split
- Evaluate on a test set
- Save the trained model

---

## Results (Baseline)

From the provided run:
- **Test Accuracy:** ~**0.82**
- Training included accuracy and validation accuracy plotting across epochs.

> Results will vary based on dataset size, quality, and class balance.

## Next Steps

### 1) Build a simple Streamlit app (front end)
Create a lightweight UI so users can upload an image and get a prediction (Real vs Fake).

**Planned features:**
- Image upload (`.jpg/.png`)
- Display uploaded image
- Run model inference and show:
  - Predicted class (Real/Fake)
  - Confidence score (sigmoid probability)
- Optional: batch upload + downloadable results

---

## Collaboration

This project was developed in collaboration with a teammate.  
My primary contributions included:

- Designing and training the CNN architecture in TensorFlow/Keras  
- Building the image preprocessing pipeline with OpenCV  
- Documenting the process  
- Saving and preparing the model for future deployment

The project was developed jointly, with shared responsibilities across data preparation, experimentation, and documentation.

---

### 2) Improve performance with hyperparameter tuning
Focus on improving generalization and accuracy beyond the baseline CNN.
