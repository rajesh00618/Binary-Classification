# Binary Classification using Deep Neural Networks

## Overview
This project implements a deep learning model for binary classification using TensorFlow and Keras.  
The Heart Disease dataset was used to demonstrate an end-to-end workflow including EDA, preprocessing, model training, evaluation, and visualization.

## Dataset
- Source: Kaggle – Heart Disease Dataset
- Target: Presence of heart disease (binary)

## Model Architecture
- Input layer matching feature dimensions
- Hidden layers: 64 → 32 → 16 neurons
- Activation: ReLU (hidden layers)
- Output: 1 neuron with Sigmoid activation

## Training Strategy
- Loss: Binary Crossentropy
- Optimizer: Adam
- Callbacks:
  - EarlyStopping (patience = 10)
  - ModelCheckpoint (best validation loss)

## Results
| Metric | Score |
|------|------|
| Accuracy | ~ 0.97 |
| Precision | ~ 0.99 |
| Recall | ~ 0.96 |
| F1-score | ~ 0.97 |
| ROC-AUC | ~ 0.99 |

## Files
- `notebook.ipynb` – Full implementation
- `model/best_model.h5` – Saved model
- `requirements.txt` – Dependencies

## How to Run
```bash
pip install -r requirements.txt
jupyter notebook
