# 🌾 Crop Recommendation System using Machine Learning

A beginner-friendly agriculture ML project that recommends a crop from soil and environmental conditions using a Random Forest classifier.

## Features
- Nitrogen (N)
- Phosphorus (P)
- Potassium (K)
- Temperature
- Humidity
- Soil pH
- Rainfall

## Project structure

```text
crop-recommendation-ml/
├── crop_dataset.csv
├── crop_recommendation_model.pkl
├── train_model.py
├── predict.py
├── requirements.txt
├── README.md
└── .gitignore
```

## Important note about the included dataset

The included `demo_crop_dataset.csv` is **synthetic demonstration data** so the project can run immediately. For a real college project, replace it with a genuine crop-recommendation dataset and retrain the model.

Your real CSV should contain these columns:

`N, P, K, temperature, humidity, ph, rainfall, label`

## Run the project

### 1. Install dependencies

```bash
pip install -r requirements.txt
```

### 2. Train the model

```bash
python train_model.py
```

This creates/updates:

`crop_recommendation_model.pkl`

### 3. Make a prediction

```bash
python predict.py
```

## Model

Algorithm: **Random Forest Classifier**

The model uses 200 decision trees and a fixed random state for reproducibility.

The demo model's test accuracy is approximately **93.6%**. This number is only for the synthetic demonstration dataset and should NOT be presented as real-world agricultural accuracy.

## GitHub

Upload the source code, dataset, README and model file to your GitHub repository.

## Future improvements

- Add a Streamlit web interface
- Compare Random Forest with Decision Tree and KNN
- Add feature importance graphs
- Use a real agricultural dataset
- Add fertilizer recommendation
- Add irrigation advice
