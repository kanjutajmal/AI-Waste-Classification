# Waste Image Classification Using CNN

A waste image classification system built using a Convolutional Neural Network (CNN) with TensorFlow/Keras. The project classifies waste images into two categories: **organic** and **recyclable**. It includes model training, evaluation (accuracy, precision, recall, F1-score, confusion matrix), and single-image prediction in a Jupyter Notebook.

Dataset: [Waste Classification Data (Kaggle)](https://www.kaggle.com/datasets/techsash/waste-classification-data)

## Project Files

| File | Purpose |
|------|---------|
| `waste_classification.ipynb` | Complete notebook: load data, train, evaluate, save model, predict |
| `requirements.txt` | Python libraries needed |
| `results/` | Saved graphs and metrics |
| `models/` | Saved trained model |

## How to Run

1. Download the dataset from Kaggle and extract it into a folder named `dataset` so that it contains `TRAIN/` and `TEST/` (each with `O/` and `R/` sub-folders).
2. Install the libraries:
   ```
   pip install -r requirements.txt
   ```
3. Open the notebook and run all cells:
   ```
   jupyter notebook waste_classification.ipynb
   ```

## Model

Input 128 x 128 RGB image, then 3 x (Conv2D + MaxPooling), Flatten, Dense(128) + Dropout(0.5), and a Sigmoid output. Optimizer: Adam. Loss: binary cross-entropy.

## Results

Add your final test accuracy, precision, recall, F1-score and confusion matrix here after training.

## Disclaimer

This project is for educational purposes only.
"# AI-Waste-Classification" 
