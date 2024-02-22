# README for Machine Learning Classification and PageRank Algorithm Script

This README provides an overview and usage guide for a Python script that encompasses two distinct machine learning tasks: logistic regression-based classification and the implementation of the PageRank algorithm for ranking nodes in a network. The script demonstrates the application of gradient descent for logistic regression and eigenvalue decomposition for PageRank.

## Part 1: Logistic Regression for Binary Classification

### Overview

The script begins with loading training data for a binary classification task, visualizing it, and then applying logistic regression to find a decision boundary. It includes the calculation of the gradient of the logistic loss function, updating weights using gradient descent, and visualizing the resulting decision boundary.

### Prerequisites

- Python 3.x
- NumPy
- Matplotlib
- pickle

### Key Components

- **Data Loading and Visualization**: Loads training data from a pickle file and visualizes it using Matplotlib.
- **Gradient Calculation**: Implements a function to calculate the gradient of the logistic loss function.
- **Gradient Descent Optimization**: Applies gradient descent to minimize the logistic loss and updates the model weights accordingly.
- **Decision Boundary Visualization**: Visualizes the training data with the learned decision boundary.
- **Error Rate Calculation**: Computes and displays the error rate of the classification model.

### Usage

1. Ensure all required libraries are installed using pip:

```bash
pip install numpy matplotlib
```

2. Place your `classifier_data.pkl` file in the same directory as the script.
3. Run the script to train the logistic regression model and visualize the results.

## Part 2: PageRank Algorithm Implementation

### Overview

Following the classification task, the script implements the PageRank algorithm to rank nodes (Wikipedia pages) based on their importance within a network defined by a set of edges (links between pages).

### Prerequisites

- Python 3.x
- NumPy
- SciPy

### Key Components

- **Data Loading**: Reads node and edge data from CSV files to construct the adjacency matrix of the network.
- **Adjacency Matrix Construction**: Constructs an adjacency matrix representing the network of nodes and their connections.
- **PageRank Algorithm**: Applies modifications to the adjacency matrix to prevent rank sinks and calculates the PageRank scores using eigenvalue decomposition.

### Usage

1. Install required libraries (if not already installed from Part 1):

```bash
pip install numpy scipy
```

2. Place your `wisconsin_edges.csv` and `wisconsin_nodes.csv` files in the same directory as the script.
3. Run the script to compute and print the PageRank scores of the nodes.

## Notes

- **Data Files**: Ensure that `classifier_data.pkl`, `wisconsin_edges.csv`, and `wisconsin_nodes.csv` are correctly formatted and located in the same directory as the script.
- **Visualization**: The script uses Matplotlib for visualization. Ensure you are in an environment where GUI windows can be opened, or adjust the script for inline plotting if using Jupyter Notebooks.
- **PageRank Computation**: The PageRank algorithm is implemented using sparse matrix operations from SciPy for efficiency. The script demonstrates a basic version of PageRank and might require adjustments for larger or more complex networks.

This script provides a practical introduction to two widely used machine learning and data analysis techniques: logistic regression for classification and the PageRank algorithm for network analysis.
