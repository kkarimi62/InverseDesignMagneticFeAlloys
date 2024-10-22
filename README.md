# Soft Magnetic Alloys: Machine Learning-Based Multi-Objective Optimization and Uncertainty Quantification
This repository presents a machine learning-based approach for the multi-objective optimization, prediction, and uncertainty quantification of soft magnetic alloys. The study focuses on the composition and processing parameters of these alloys, applying various machine learning models and optimization techniques to predict and enhance the magnetic properties of interest.

<img src="workFlow.jpg" width="800"/>

## Key Features

- **Data Utilization:** Analysis of elemental compositions and processing parameters to predict properties like Magnetic Saturation (Bs) and Curie Temperature (Tc).
- **Machine Learning Models:** Applied Ridge Regression, Support Vector Machines (SVM), CatBoost, Gaussian Process Regression (GPR), K-Nearest Neighbors (KNN), and Dense Neural Networks to predict the material properties.
- **Prediction Results:** Model performance is evaluated using metrics such as the Root Mean Square Error (RMSE) to ensure the accuracy of property predictions.

## Requirements

- Python 3.x
- TensorFlow
- DeepMind’s GNN library
- Other Python packages (see `gnnPolyCryst.ipynb`)

## Installation

1. Clone this repository:
    ```bash
    git clone git@github.com:kkarimi62/polyGNN.git
    cd polyGNN
    ```

## Usage

1. **Prepare Data:**
   - Ensure you have EBSD maps and nanoindentation data in the correct format.
   - Place your data files in the `data/` directory.

2. **Train the Model:**
   - Execute Jupyter notebook `gnnPolyCryst.ipynb`
