# Predictive Maintenance for Trains and Aircraft

## Project Overview

This project investigates machine learning and neural network
techniques for predictive maintenance in transportation systems.

The project consists of two main parts: representation learning
for train sensor data and sequence learning for aircraft engine
Remaining Useful Life (RUL) prediction.

## Part A - Representation Learning (Trains)

Dataset: MetroPT-3 Train Sensor Dataset

### Implemented Methods

- Principal Component Analysis (PCA)
- Linear Autoencoder
- Self-Organising Map (SOM)
- Anomaly Detection

### Results

| Evaluation Metric | Result |
|---|---:|
| PCA Explained Variance | 59.14% |
| PCA Reconstruction MSE | 0.388070 |
| Autoencoder Reconstruction MSE | 0.388751 |
| SOM Quantisation Error | 0.491853 |
| Potential Anomalies | 473 |
| Potential Anomaly Percentage | 4.73% |

## Part B - Sequence Learning (Aircraft)

Dataset: NASA C-MAPSS FD001

### Implemented Models

- Simple Recurrent Neural Network (RNN)
- Long Short-Term Memory (LSTM)
- Mean Baseline Model

### Model Performance

| Metric | Simple RNN | LSTM | Mean Baseline |
|---|---:|---:|---:|
| MAE | 17.9632 | 16.8332 | 36.6155 |
| MSE | 627.4072 | 573.6817 | 2096.7742 |
| RMSE | 25.0481 | 23.9517 | 45.7905 |
| R2 Score | 0.6367 | 0.6678 | -0.2142 |
| NASA Score | 5460.035 | 13490.561 | 73242.911 |

LSTM achieved better conventional regression performance,
while Simple RNN achieved a lower NASA asymmetric score.

## Repository Files

| File | Description |
|---|---|
| AMLNN_AS2.ipynb | Complete project notebook |
| aircraft_rnn.keras | Trained RNN model |
| aircraft_lstm.keras | Trained LSTM model |
| aircraft_scaler.pkl | Feature standardisation scaler |
| aircraft_configuration.pkl | Model configuration |
| model_comparison.csv | Model evaluation results |
| rul_predictions.csv | Actual and predicted RUL values |
| requirements.txt | Required Python libraries |

## Technologies Used

- Python
- Google Colab
- TensorFlow and Keras
- Scikit-learn
- NumPy
- Pandas
- Matplotlib
- Seaborn
- MiniSom

## Datasets

- MetroPT-3 Train Sensor Dataset:
  https://archive.ics.uci.edu/dataset/791/metropt+3+dataset

- NASA C-MAPSS Turbofan Engine Degradation Dataset (FD001)

The original datasets are not included in this repository
because of their size.

## How to Run the Project

1. Download the required datasets.
2. Open AMLNN_AS2.ipynb in Google Colab.
3. Install the required Python libraries.
4. Connect Google Drive and configure the dataset paths.
5. Run the notebook cells in sequential order.

## Conclusion

The findings demonstrate the potential of representation
learning and recurrent neural networks to identify unusual
operating patterns and predict equipment degradation.

Further optimisation and real-world validation are required
before practical deployment.

## Academic Information

Module: Advanced Machine Learning and Neural Networks

Assignment: Assignment 2

Programme: BSc (Hons) Data Science

University: University of Hertfordshire

This project was developed for academic purposes.
