# Soft Magnetic Alloys: Machine Learning-Based Multi-Objective Optimization and Uncertainty Quantification
This repository presents a machine learning-based approach for the multi-objective optimization, prediction, and uncertainty quantification of soft magnetic alloys. The study focuses on the composition and processing parameters of these alloys, applying various machine learning models and optimization techniques to predict and enhance the magnetic properties of interest.

<img src="workFlow.jpg" width="800"/>

## Key Features

- **Data Utilization:** Analysis of elemental compositions and processing parameters to predict properties like Magnetic Saturation (Bs) and Curie Temperature (Tc).
- **Machine Learning Models:** Applied Ridge Regression, Support Vector Machines (SVM), CatBoost, Gaussian Process Regression (GPR), K-Nearest Neighbors (KNN), and Dense Neural Networks to predict the material properties.
- **Bayesian Optimization:** Implemented inverse design and property maximization strategies using a Bayesian approach to refine alloy compositions.
- **Uncertainty Quantification:** Utilized Bayesian strategies to analyze the posterior distribution of key variables, such as Fe composition, and assess their impact on property uncertainty.
- **Constrained Optimization:** Applied refined optimization techniques with constraints, incorporating the Pareto front to guide trade-offs and balance multiple design goals.

## Key Findings:

- **Optimization Results:** Excluding the Tx constraint, Pareto front analysis indicates a trade-off between maximizing Bs and Tc. When the constraint is applied, it may be possible to optimize both properties simultaneously.
- **Uncertainty Quantification:** Bayesian analysis underscores the influence of fluctuations in Fe composition on the uncertainty of Bs, demonstrating the necessity of precise composition control to reduce variance.
- **Data Limitations:** The current dataset lacks the depth needed to fully capture the complex interplay between composition and processing conditions, highlighting the need for more comprehensive data to develop robust alloy designs.
- **Model Refinement:** Further fine-tuning of machine learning models during the optimization process is expected to enhance prediction accuracy.
- **Real-World Validation:** Future work should incorporate experimental validation of the predicted alloy compositions to evaluate the practical effectiveness of the models in real-world applications.

## Requirements

- Python 3.x
- TensorFlow
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
