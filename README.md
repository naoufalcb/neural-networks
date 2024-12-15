# Neural Networks

This repository contains two essential algorithms implemented from scratch in Python: **Gradient Descent** and a **Neural Network for Predicting Student Admissions**. The aim is to provide an educational example of how these algorithms work, step-by-step.

## Table of Contents

- [Overview](#overview)
- [1. Implementing the Gradient Descent Algorithm](#1-implementing-the-gradient-descent-algorithm)
- [2. Predicting Student Admissions with Neural Networks](#2-predicting-student-admissions-with-neural-networks)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

---

## Overview

This repository demonstrates how the **Gradient Descent Algorithm** can be used for binary classification tasks, and also shows the implementation of a basic neural network to predict student admissions based on GRE scores, GPA, and class rank.

---

## 1. Implementing the Gradient Descent Algorithm

The first notebook focuses on implementing the **Gradient Descent** algorithm for binary classification. The algorithm is used to classify a simple dataset into two classes while visualizing the decision boundary as it evolves over time.

### Key Functions Implemented:
- **sigmoid**: Maps inputs to a range between 0 and 1.
- **output_formula**: Computes the model’s prediction based on weights and inputs.
- **error_formula**: Calculates the error for the prediction.
- **update_weights**: Performs weight updates using the gradient descent formula.

### Features:
- **Data Visualization**: Visualizes the dataset and decision boundaries.
- **Interactive Learning**: Implement core functions and see their effects immediately.
- **Error Plotting**: Visualizes how the error function decreases over epochs.

### Usage:

- Load your dataset into the `data.csv` file.
- Execute the code cells to train the model, visualize the decision boundary, and plot the error curve.
- Observe how the decision boundary improves as the algorithm iterates through more epochs.

```bash
# To train the model:
train(X, y, epochs, learnrate, True)
```

---

## 2. Predicting Student Admissions with Neural Networks

This notebook uses a **Neural Network** to predict student admissions to graduate school at UCLA based on their GRE scores, GPA, and class rank.

### Dataset:
The dataset used for this project contains the following features:
- GRE scores (Test)
- GPA scores (Grades)
- Class rank (1-4)

### Data Processing:
- **One-hot Encoding**: Class rank is one-hot encoded to include it as a feature.
- **Data Scaling**: GRE scores are scaled by dividing by 800, and GPA scores are scaled by dividing by 4.0.
- **Data Splitting**: The data is split into training and testing datasets.

### Model Workflow:
- **Training**: The model is trained using the processed features and the target (admission status).
- **Prediction**: The neural network predicts whether a student will be admitted based on the input features.

---

## Installation

To run the notebooks, you'll need to have Python and the following libraries installed:

- `numpy`
- `pandas`
- `matplotlib`

You can install these dependencies using `pip`:

```bash
pip install numpy pandas matplotlib
```

---

## Usage

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/neural-networks.git
    cd neural-networks
    ```

2. Open the notebooks (`gradient_descent.ipynb` and `student_admissions.ipynb`) in your Jupyter Notebook or any Python IDE of your choice.

3. Follow the instructions inside each notebook to execute the code and visualize the results.

---

## Contributing

Contributions are welcome! If you'd like to improve the code or suggest features, please feel free to fork the repository and submit a pull request. If you find any issues, you can open an issue on the GitHub page.

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Feel free to modify this template further based on your repository details.
