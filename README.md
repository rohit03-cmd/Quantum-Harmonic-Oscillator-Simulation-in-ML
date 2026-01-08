# Quantum Harmonic Oscillator Simulation via Machine Learning

## 🌌 Project Overview
This project simulates a **Quantum Harmonic Oscillator (QHO)** by predicting the ground-state energy ($E_0$) based on physical parameters like mass ($m$) and angular frequency ($\omega$). By leveraging a Deep Neural Network (DNN), the model learns to approximate the solutions to the time-independent Schrödinger equation ($H\psi = E\psi$) without the need for traditional numerical integration.

## 🚀 Key Features
* **Physics-Informed Data Generation:** Generates a dataset of 10,000 samples based on the analytical ground-state formula: $E_0 = \frac{1}{2}\hbar\omega$ (with $\hbar = 1$).
* **Deep Learning Model:** A sequential neural network architecture with three hidden layers (64, 32, and 16 neurons) using ReLU activation.
* **Interactive GUI:** A Tkinter-based graphical interface for loading datasets, training models, visualizing training loss, and predicting energy for custom user inputs.
* **Analytical Validation:** Integration with **SymPy** to provide real-time error analysis by comparing ML predictions against exact analytical results.

## 📊 Performance (XYZ Formula Results)
Based on Jeff Su's "Golden Rules" for impact, the model achieves the following:
* **High Accuracy:** Achieved a **99.99% R² score** and a Mean Squared Error (MSE) of **0.000002** by optimizing a multi-layer perception architecture.
* **Low Predictive Error:** Reduced absolute error to **<0.002** for unseen test cases as measured by analytical comparison with the exact Schrödinger solution.
* **Optimized Training:** Minimized training convergence time through the implementation of an **Early Stopping** callback, preventing overfitting while maintaining high generalization.

## 🛠️ Technical Stack
* **Languages:** Python
* **Libraries:** TensorFlow/Keras, NumPy, Pandas, Scikit-Learn
* **Visualization:** Matplotlib
* **Symbolic Math:** SymPy
* **GUI:** Tkinter

## 📁 Project Structure
```text
├── Quantum Harmonic Oscillators.ipynb     # Main simulation & training logic
├── GUI for Quantum Harmonic Oscillators.ipynb # Interactive GUI implementation
├── quantum_harmonic_oscillator_data.csv   # Generated training dataset
└── README.md                              # Documentation
