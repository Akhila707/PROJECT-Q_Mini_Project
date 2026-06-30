# 🌌 Quantum Randomness Laboratory

This repository contains the implementation of **Mini Project 1: Quantum Randomness Laboratory**, developed as part of the **PROJECT-Q Challenge (Day 5)**. The project demonstrates the practical and conceptual differences between classical pseudo-randomness and true quantum randomness through physical wave-function collapse.

---

## 🛠️ Project Structure

All project modules, visualizations, and statistical tracking are completely integrated into a single, self-contained Jupyter Notebook:

```text
Quantum-Randomness-Lab/
│
└── quantum_randomness.ipynb   # Complete interactive Quantum Lab notebook
⚙️ Setup and Prerequisites
1. Environment Activation
Ensure your Python virtual environment is activated before running the notebook:
2. Dependencies
The notebook utilizes the following libraries:

Qiskit & Qiskit-Aer: Constructing and simulating the quantum circuit.

Matplotlib: Plotting empirical state frequencies.

NumPy: Extracting mathematical statistical parameters.

If needed, re-verify your environment packages:
🔬 Implementation Overview Inside the Notebook1. Quantum Random Number Generation (QRNG)The core engine creates a single-qubit quantum circuit, applies a Hadamard (H) Gate to establish an equal superposition state ($|\psi\rangle = \frac{1}{\sqrt{2}}|0\rangle + \frac{1}{\sqrt{2}}|1\rangle$), and executes single-shot measurements (shots=1) to simulate true physical wave-function collapse.2. Empirical Visualization PipelineGenerates an expanded data stream of 100 isolated quantum random bits and maps out the sample frequency distribution using a clean bar chart layout to observe the convergence behavior toward a 50/50 split.3. Statistical Analysis EngineExtracts mathematical parameters across the quantum iterations utilizing NumPy to review:Total counts of state $|0\rangle$ and state $|1\rangle$.Arithmetic Mean ($\mu$) approaching $0.5$.Standard Deviation ($\sigma$) mapping the dispersion of true superposition randomness.4. Classical Random BaselineGenerates a parallel control array using standard seed-based mathematical formulas (random.randint) to provide a clear benchmark comparing predictable, algorithmic sequences against true physical quantum uncertainty.
