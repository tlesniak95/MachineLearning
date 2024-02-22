# README for Dimensionality Reduction and Visualization Script

This README document provides an overview and instructions for using a Python script focused on dimensionality reduction and data visualization techniques. The script explores data structuring, low-rank approximation, mean subtraction, Singular Value Decomposition (SVD), and the visualization of data and its principal components in a three-dimensional space.

## Overview

The script is divided into several sections, each addressing different aspects of data analysis and visualization:

- **2a & 2b:** Discussion on data structure and the concept of low-rank approximation for reducing data to a lower dimension.
- **Interactive 3D Plotting:** Utilizing `%matplotlib notebook` for interactive 3D visualization of the data.
- **Data Loading and Visualization:** Loading data from a CSV file and visualizing it in 3D space.
- **Mean Subtraction (Zero-Centering):** Adjusting data to have a mean of zero, essential for PCA analysis.
- **Principal Component Analysis (PCA):** Using SVD to identify principal components of the data.
- **Dimensionality Reduction:** Visualizing the effect of projecting data onto principal components.
- **Low-Rank Approximations:** Demonstrating the use of singular values and vectors for data approximation and visualization of these approximations.

## Prerequisites

Ensure you have the following Python packages installed:

- NumPy
- Matplotlib
- SciPy

You can install these packages using pip if you haven't already:

```bash
pip install numpy matplotlib scipy
```

## Instructions

1. **Prepare Your Environment:**
   - Ensure all required packages are installed.
   - Place your data file (`sdata.csv`) in the same directory as the script.

2. **Run the Script:**
   - The script can be executed as a whole if you're using an interactive environment like Jupyter Notebooks, which supports `%matplotlib notebook` for 3D interactive plots.
   - If running in a non-interactive environment, you might need to modify `%matplotlib notebook` to `%matplotlib inline` or adjust according to your setup.

3. **Explore the Data:**
   - The script will first display the original data in 3D space.
   - After subtracting the mean, it will show the zero-centered data.
   - It then uses SVD to find and plot the first principal component.

4. **Dimensionality Reduction Visualization:**
   - Visualizes how data can be approximated by projecting it onto the first principal component and then extends this to a rank-2 approximation using the first two principal components.

5. **Rank-2 Approximation and Error Calculation:**
   - Finally, the script calculates and displays the Frobenius norm of the residual matrix from the rank-2 approximation, illustrating the amount of variance captured by the first two principal components.

## Notes

- **Data File:** This script assumes the presence of a file named `sdata.csv`, containing three-dimensional data points.
- **Interactive Plots:** If interactive rotation of graphs is not working, ensure you're running the script in an environment that supports `%matplotlib notebook`.
- **Customization:** You may need to adjust file paths, plot dimensions, or other parameters based on your specific requirements or data.

This script provides a practical introduction to key concepts in data analysis, including dimensionality reduction, PCA, and SVD, along with interactive visualization techniques to explore and understand high-dimensional data.
