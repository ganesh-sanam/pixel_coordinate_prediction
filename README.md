# Pixel Coordinate Prediction using Deep Learning

## Problem Statement
Predict the (x, y) coordinates of a single pixel with value 255 in a 50x50 grayscale image,
where all other pixels are 0. The position of the active pixel is randomly assigned.

## Approach
- A synthetic dataset is generated where each image contains exactly one active pixel.
- Images are flattened into 2500-dimensional vectors.
- A Multi-Layer Perceptron (MLP) is used to regress the (x, y) coordinates.
- Inputs and outputs are normalized to improve training stability.

## Dataset
- Image size: 50 x 50
- Input shape: (N, 2500)
- Output shape: (N, 2)
- Labels represent the ground truth pixel coordinates.

## Model
- Type: Multi-Layer Perceptron (MLP)
- Loss function: Mean Squared Error (MSE)
- Optimizer: Adam

## Results
- Training and validation loss converge smoothly.
- Predicted coordinates closely match ground truth.
- Visualization confirms accurate localization of the active pixel.

## How to Run
1. Install dependencies:
   pip install -r requirements.txt
2. Open and run the notebook:
   pixel_coordinate_prediction.ipynb

## Notes
This project demonstrates a simple and effective deep learning approach for coordinate regression.
