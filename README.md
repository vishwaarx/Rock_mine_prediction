# Sonar Object Classification

This repository contains a machine learning project that classifies sonar signals as either rocks or mines using a logistic regression model. The dataset used is the Sonar dataset, which contains 60 features representing the intensity of sound waves at different angles.

## Project Overview

The goal of this project is to accurately classify sonar signals as either a rock or a mine using Logistic Regression. This classification is essential in differentiating between objects detected by sonar devices.

## Dataset

- **Dataset Name**: Sonar Dataset
- **Source**: The dataset can be found on [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/connectionist+bench+%28sonar,+mines+vs.+rocks%29).
- **Features**: 60 continuous attributes representing energy in various frequency bands.
- **Target**: Binary classification where 'R' indicates a Rock and 'M' indicates a Mine.

## Project Structure

- **`sonar_data.csv`**: The dataset used for training and testing.
- **`sonar_classification.ipynb`**: Jupyter notebook containing code for data preprocessing, model training, and evaluation.
- **`README.md`**: This file.

## Workflow

1. **Data Preprocessing**: 
    - Data was loaded and basic statistical analysis was performed.
    - Features and target variables were separated, and the data was split into training and testing sets using stratified sampling to maintain class balance.

2. **Model Training**:
    - A logistic regression model was trained on the dataset.
    - Achieved an accuracy of **83.6%** on the training set and **76.1%** on the test set.

3. **Evaluation**:
    - The model was evaluated using accuracy as the performance metric.
    - Predictions were made on unseen data, showing how well the model differentiates between rocks and mines.

4. **Prediction on New Data**:
    - A real-time prediction example is provided where a new sonar signal is classified as either a rock or a mine.

## Results

- **Training Accuracy**: 83.6%
- **Test Accuracy**: 76.1%

## How to Use

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/Sonar-Object-Classification.git
    ```
2. Install the necessary dependencies:
    ```bash
    pip install -r requirements.txt
    ```
3. Run the notebook:
    Open `sonar_classification.ipynb` to run the model and follow the code step by step to understand the data preprocessing and model training process.

## Future Work

- Experiment with other classification algorithms such as Random Forest, SVM, or Neural Networks.
- Improve model accuracy by applying feature selection or hyperparameter tuning.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
