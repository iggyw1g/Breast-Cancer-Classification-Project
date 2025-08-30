# Breast Cancer Classification Analysis

An end-to-end machine learning project to classify breast cancer tumors as malignant or benign. This repository contains the data analysis, model training, and comparative evaluation of three different classification algorithms.

[![Build Status](https://img.shields.io/badge/build-passing-brightgreen)](https://github.com/[your-username]/[your-repo])
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Python](https://img.shields.io/badge/Python-3776AB.svg?style=flat&logo=python&logoColor=white)](https://www.python.org/)
[![Scikit-Learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=flat&logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)

## Table of Contents

- [About The Project](#about-the-project)
- [Analysis Overview](#analysis-overview)
- [Tech Stack](#tech-stack)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)
- [Contributors](#contributors)

---

## About The Project

The goal of this project is to accurately predict whether a breast cancer tumor is **malignant** or **benign** based on a set of digitized image features. Early and accurate diagnosis is critical for patient outcomes, making this a vital application of machine learning.

This project walks through the entire data science workflow, including:

- **Loading and cleaning** the dataset.
- **Exploring and visualizing** the data to understand feature relationships.
- **Training and comparing** three distinct classification models.
- **Evaluating** the models with a focus on metrics that are critical for medical diagnoses, such as **Recall**.

The ultimate objective is to identify the most effective and reliable model for this classification task.

---

## Analysis Overview

- 📊 **Exploratory Data Analysis (EDA):** Performed initial analysis to understand the data distribution and used correlation heatmaps to identify relationships between features.
- ⚙️ **Feature Engineering & Selection:** Analyzed different subsets of features (mean, worst) and used Random Forest's built-in feature importance to identify the most predictive variables.
- 🧠 **Model Training:** Implemented and trained three powerful classification models:
  1.  **Logistic Regression**
  2.  **Support Vector Machine (SVM)**
  3.  **Random Forest Classifier**
- 📈 **Model Evaluation:** Performed a robust evaluation using K-Fold Cross-Validation, Confusion Matrices, and a detailed Classification Report. The primary focus was on maximizing the recall for malignant cases (Class 1) to minimize dangerous false negatives.

---

## Tech Stack

This project was developed entirely in Python within a Jupyter Notebook environment.

| Component              | Technology / Library                                                                                                                                                                                                                     |
| :--------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Language**           | ![Python](https://img.shields.io/badge/Python-3776AB.svg?style=for-the-badge&logo=python&logoColor=white)                                                                                                                                |
| **Data Manipulation**  | ![NumPy](https://img.shields.io/badge/NumPy-013243.svg?style=for-the-badge&logo=numpy&logoColor=white) ![Pandas](https://img.shields.io/badge/Pandas-150458.svg?style=for-the-badge&logo=pandas&logoColor=white)                         |
| **Data Visualization** | ![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black) ![Seaborn](https://img.shields.io/badge/Seaborn-%23023e8a.svg?style=for-the-badge&logo=Seaborn&logoColor=white) |
| **Machine Learning**   | ![Scikit-Learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)                                                                                                          |
| **Environment**        | ![Jupyter](https://img.shields.io/badge/Jupyter-F37626.svg?style=for-the-badge&logo=Jupyter&logoColor=white)                                                                                                                             |

---

## Getting Started

To get a local copy up and running, follow these simple steps.

### Prerequisites

You will need Python 3 and Pip installed on your system.

### Installation

1. **Clone the repository:**
   ```sh
   git clone https://github.com/iggyw1g/MLProj
   ```
2. **Navigate into the project directory:**
   ```sh
   cd MLProj
   ```
3. **Install the required libraries:**
   - It is recommended to use a virtual environment.
   ```sh
   pip install pandas matplotlib seaborn numpy scikit-learn jupyter
   ```
4. **Run the Jupyter Notebook:**
   ```sh
   jupyter notebook finalproject.ipynb
   ```

## Results

After a comprehensive evaluation of all three models, the Support Vector Machine (SVM) with a linear kernel was identified as the top-performing model.

- SVM (Linear Kernel): Achieved the best balance of precision and recall, demonstrating a strong ability to distinguish between malignant and benign tumors with high confidence. The linear nature of the model suggests that the feature space is largely linearly separable.
- Random Forest: Also performed exceptionally well, providing a robust model and valuable insights through its feature importance scores.
- Logistic Regression: Served as a strong baseline but was ultimately outperformed by the more complex ensemble and margin-based models.

The final conclusion emphasizes the importance of recall for malignant cases, where the SVM model proved highly effective, successfully identifying 93% of all malignant tumors in the test set.

## Contributing

Contributions are welcome! If you have suggestions for improving the analysis, please feel free to fork the repo and create a pull request.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/NewAnalysis`)
3. Commit your Changes (`git commit -m 'Add some NewAnalysis'`)
4. Push to the Branch (`git push origin feature/NewAnalysis`)
5. Open a Pull Request

## License

Distributed under the MIT License. See `LICENSE` file for more information.

## Contributors

- Riju Pant - https://github.com/Rp0115
- Alisa Sumwalt - https://github.com/iggyw1g
- Andrew ZiYu Wang - https://github.com/20wangaz2

Project Link: https://github.com/iggyw1g/MLProj
