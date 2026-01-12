# Numpy — Hands-on Learning Material

![Python](https://img.shields.io/badge/Python-3.8%2B-3776AB?logo=python&logoColor=white) ![NumPy](https://img.shields.io/badge/NumPy-Array%20Library-013243?logo=numpy&logoColor=white) ![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white) ![VS Code](https://img.shields.io/badge/Editor-VS%20Code-007ACC?logo=visual-studio-code&logoColor=white) ![License](https://img.shields.io/badge/License-MIT-blue)

This repository contains hands-on learning material for NumPy, focusing on numerical computing, array operations, statistics, and matrix manipulation with simple examples. The main content is provided as a Jupyter Notebook: `numpy.ipynb`.

Table of Contents
- **About**
- **Features**
- **Requirements**
- **Installation**
- **Quickstart Examples**
  - Creating arrays
  - Inspecting arrays (dtype, shape)
  - Indexing & slicing
  - Arithmetic & broadcasting
  - Aggregation / statistics
  - Linear algebra (matrix ops)
  - Random sampling
- **Using the Notebook**
- **Suggested Learning Path & Exercises**
- **Contributing**
- **License**
- **Files in this repository**
- **Contact**

## **About**
This repository is designed for learners who want to build a practical foundation in NumPy. The notebook walks through core concepts with short, runnable examples and brief explanations. Use the notebook for interactive exploration and this README for a quick reference.

## **Features**
- Introductory examples for NumPy fundamentals
- Array creation, manipulation, and indexing
- Aggregation and statistics (mean, sum, std, percentiles)
- Matrix operations and linear algebra examples
- Random number generation and sampling
- A single self-contained Jupyter notebook for interactive learning: `numpy.ipynb`

## **Requirements**
- Python 3.8+ recommended (Python 3.7+ should also work)
- pip or conda to install packages
- Jupyter Notebook or JupyterLab to run the notebook interactively

## **Installation**

Using pip:
```bash
python -m pip install --upgrade pip
pip install numpy jupyter
```

Using conda:
```bash
conda create -n numpy-tutorial python=3.9 -y
conda activate numpy-tutorial
conda install numpy jupyter -y
```

## **Quickstart Examples**
Below are a few compact, essential examples. For full runnable examples and explanations, open `numpy.ipynb`.

Import NumPy (always start with this):
```python
import numpy as np
```

Creating arrays (short example):
```python
a = np.array([1, 3, 4])       # 1D array
m = np.array([[1, 2, 3],      # 2D array (matrix)
              [4, 5, 6]])
```

Inspecting arrays and basic attributes (describe rather than show many code blocks):
- dtype: data type of elements (e.g., float64, int64)
- shape: tuple describing array dimensions
- ndim: number of dimensions
- size: total number of elements

Indexing & slicing:
- Use standard Python-style indexing for 1D arrays.
- For 2D arrays: `arr[row, col]`, slice rows/columns with `:` and use boolean indexing for filtering.

Arithmetic & broadcasting:
- Elementwise operations (e.g., `a + b`) operate element-by-element.
- Broadcasting lets you combine arrays of different shapes in a consistent manner (e.g., adding a 1D vector to each row of a 2D matrix).

Aggregation / statistics:
- Common operations: `mean()`, `sum()`, `std()`, `median`, `percentile`.
- Most aggregation functions accept an `axis` argument to reduce along specific dimensions.

Linear algebra:
- Matrix multiplication: `A @ B` or `np.matmul(A, B)`.
- Transpose: `A.T`.
- Inverse / solve: use `np.linalg.inv` (careful: only for invertible matrices) and `np.linalg.solve` for linear systems.

Random sampling:
- Random integers: `np.random.randint(low, high, size=...)`
- Standard normal samples: `np.random.normal(loc=0.0, scale=1.0, size=...)`

Note: Many small code examples and exercises are available in `numpy.ipynb` — this README keeps examples minimal and points you to the notebook for hands-on practice.

## **Using the Notebook**
- Install Jupyter (see Installation).
- Start Jupyter Notebook from the repository root:
  ```bash
  jupyter notebook
  ```
  or for JupyterLab:
  ```bash
  jupyter lab
  ```
- Click on `numpy.ipynb` to open the interactive tutorial.
- Run the cells step-by-step. Modify examples to explore behavior and experiment with shapes, dtypes, and operations.

## **Suggested Learning Path & Exercises**
1. Read the first section of the notebook to understand ndarray and basic array creation.
2. Practice reshaping and indexing on small arrays.
3. Recreate broadcasting examples and predict the output before running them.
4. Implement simple statistics: compute mean, variance, percentiles on synthetic datasets.
5. Solve linear algebra toy problems (matrix multiplication, solving A x = b).
6. Suggested exercises to modify in the notebook:
   - Create a 3D array and compute sums along different axes.
   - Use boolean indexing to filter arrays (e.g., select elements > threshold).
   - Compare performance of a pure Python loop vs. NumPy operations for a large array.

## **Contributing**
Contributions are welcome:
- Open an issue for suggestions, typos, or proposed changes.
- For code or content updates, fork the repo, make your changes, and open a pull request.
- Keep examples small, runnable, and well-documented.
- Please reference the notebook when adding or changing examples to keep the learning flow consistent.

## **License**
This project is licensed under the MIT License — see the included LICENSE file for details.

## **Files in this repository**
- numpy.ipynb — interactive Jupyter Notebook with examples and explanations
- README.md — this file
- LICENSE — MIT License

## **Contact**
Author: Zia ul Islam Mughal  
(See repository author on GitHub for contact links)

Happy learning — explore, experiment, and extend the notebook with your own NumPy exercises!