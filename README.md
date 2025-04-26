# Quantum-Circuits-for-Smarter-Predictions-A-New-Era-of-Linear-Regression

## Overview
In this project, we explored the potential of Quantum Machine Learning (QML) for predictive modeling by applying Quantum Linear Regression on a large-scale dataset.  
The primary focus was to investigate whether quantum-enhanced models can provide competitive performance compared to classical machine learning approaches, especially for complex, high-volume data.

---

## Problem Statement
Traditional machine learning models can face scalability or efficiency challenges when handling large, high-dimensional datasets.  
This project aims to assess whether quantum circuits — through efficient encoding and parameterization — can offer new opportunities for enhancing prediction tasks, particularly in linear regression scenarios.

---

## Dataset Details
- **Size:** 1 Lakh+ rows
- **Features:** Mix of numerical and categorical attributes
- **Target:** Continuous value prediction
- **Preprocessing Techniques:**  
  - Feature Scaling (Normalization between -1 and 1)  
  - Encoding for quantum processing  

The dataset was thoroughly cleaned and normalized to suit quantum circuit input requirements.

---

## Setup
- **Programming Language:** Python 3.10+
- **Quantum Frameworks:**  
  - Qiskit  
  - Qiskit Machine Learning  
- **Classical Libraries:**  
  - NumPy, SciPy, Scikit-Learn, Matplotlib
- **Simulator:** IBM Qiskit Aer Simulator (local CPU-based backend)
- **Optimization:** COBYLA optimizer for quantum parameter tuning

---

## Establishing the Quantum Circuit
The modeling pipeline involved designing a hybrid quantum-classical circuit:
- **Feature Map:**  
  - `ZFeatureMap` was employed to encode classical data into quantum states through parameterized rotations.
- **Ansatz:**  
  - A `RealAmplitudes` ansatz was selected to introduce trainable parameters and allow complex function mapping.
- **Circuit Composition:**  
  - The feature map and ansatz circuits were entangled to form a complete quantum circuit architecture.

Finally, the circuit was integrated into a Quantum Neural Network (QNN) using Qiskit's `EstimatorQNN`, allowing end-to-end training through classical optimization loops.

---

## Implementation Steps
1. **Data Preparation:**  
   Splitting the dataset into training and testing subsets; applying normalization and feature transformation for quantum compatibility.
2. **Quantum Model Construction:**  
   Building the feature map, ansatz, and merging them into a quantum circuit.  
   Deploying the EstimatorQNN for regression modeling.
3. **Training:**  
   Fine-tuning circuit parameters by minimizing a regression loss using a classical optimizer.
4. **Evaluation:**  
   Measuring performance on test data using Mean Squared Error (MSE) and R² metrics.

---

## Results
- **Mean Squared Error (MSE):** ~0.1691
- **Mean Absolute Error (MAE):** ~0.3946
- **R² Score:** ~0.7440
- **Key Insights:**  
  - The quantum model achieved a positive R² on a large real-world dataset, indicating effective learning and prediction capabilities.  
  - Performance was comparable to classical regression models despite using a quantum simulator.  
  - Demonstrated the feasibility of using quantum circuits for real-world-scale regression problems.

---

## Conclusion
Although quantum computing and its machine learning applications are still in the early stages of development, the results of this project demonstrate strong potential.
The model achieved a Mean Squared Error (MSE) of 0.1691, a Mean Absolute Error (MAE) of 0.3946, and an impressive R-squared (R²) score of 0.7440.
This indicates that quantum-based approaches can not only learn meaningful patterns from large datasets but also deliver competitive predictive accuracy.
With further optimization and advancements in quantum hardware, it is expected that the performance can be improved even further, opening up exciting opportunities for real-world deployment of quantum machine learning models.



