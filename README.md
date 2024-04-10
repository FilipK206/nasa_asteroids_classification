## Near-Earth Object (NEO) Classification using XGBoost

This repository contains Python code for classifying Near-Earth Objects (NEOs) as hazardous or non-hazardous using the XGBoost classification algorithm.

### Overview

The code performs the following tasks:

1. **Data Loading and Preprocessing**: The data is loaded from a CSV file named `nasa.csv` using the pandas library. Unnecessary columns are dropped, and correlation analysis is conducted to identify redundant features.

2. **Feature Engineering**: Certain columns like 'Orbiting Body' and 'Equinox' are analyzed to understand their distribution and importance. Features with low correlation or deemed redundant are dropped from the dataset.

3. **Model Training**: The dataset is split into training and testing sets using the `train_test_split` function from the `sklearn.model_selection` module. An XGBoost classifier model is initialized and trained on the training data.

4. **Model Evaluation**: The trained model's performance is evaluated on the testing data using accuracy as the evaluation metric. Additionally, feature importance is visualized using the `plot_importance` function from the `xgboost` library.

## Dependencies

- pandas
- numpy
- sklearn
- seaborn
- matplotlib
- xgboost

## Usage

1. Ensure you have all the required dependencies installed.
2. Download or clone this repository to your local machine.
3. Place your dataset file named `nasa.csv` in the repository directory.
4. Run the `neo_classification.py` script.

## File Structure

- `neo_classification.py`: Main Python script for performing NEO classification.
- `nasa.csv`: Dataset containing NEO attributes.
- `README.md`: This file, providing an overview of the project and instructions for use.

## Acknowledgements

The dataset used in this project is sourced from [Kaggle](https://www.kaggle.com/). Special thanks to Kaggle for providing valuable data for research and analysis.
