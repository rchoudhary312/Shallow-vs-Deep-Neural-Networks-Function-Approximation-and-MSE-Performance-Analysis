# Shallow vs Deep Neural Networks – Function Approximation and MSE Performance Analysis


## ABOUT THE PROJECT:
This project investigates the approximation capabilities of neural networks with different depths (1, 2, and 3 hidden layers) for a non-linear function:
  f(x) = 2 * (2 * cos²(x) - 1)² - 1
By generating synthetic data and training multiple neural networks, the project compares how depth and number of parameters affect model performance using mean squared error (MSE) as the evaluation metric.


## USE CASE EXPLANATION:
This project belongs to the domain of deep learning theory and function approximation. It explores how depth in neural networks influences the ability to learn complex non-linear functions. The work helps answer a critical model design question: when does adding depth improve performance, and when is increasing width enough? The findings are relevant to practitioners designing models for vision, NLP, and scientific applications where approximation capacity matters.


## HOW IT IS BUILT AND FULL WORKING:

1. Data Generation:

- Sampled 120,000 data points: x ~ U(-2π, 2π)

- Computed targets using the function: y = 2 * (2 * cos²(x) - 1)² - 1

- Split into 60,000 training and 60,000 testing examples

2. Neural Network Architectures:

- Trained 3 architectures:

   1. Shallow: 1 hidden layer

   2. Moderate Depth: 2 hidden layers

   3. Deep: 3 hidden layers

- Varied the number of units per layer to study model capacity

- Used ReLU activation and MSE loss

3. Training & Evaluation:

- Trained each model on the training set and evaluated on the test set

-Compared MSE performance across:

   1. Number of units per layer

   2. Total number of parameters

   3. Visualized results with performance-vs-capacity plots to benchmark how effectively each architecture approximated the function


## OUTPUT AND RESULTS OR BENCHMARKS:

- Shallow networks showed underfitting and high error even with increased width

- 2-layer networks performed better but hit a performance ceiling at medium capacity

- 3-layer deep networks achieved lower MSE using fewer parameters — demonstrating depth efficiency

- Performance curves clearly showed that deeper networks generalize better for non-linear function approximation


## SKILLS, TOOLS:
Python, NumPy, PyTorch or TensorFlow, Matplotlib, synthetic data generation, supervised learning, function approximation, MSE loss, ReLU networks

## KEYWORDS:
Deep learning, neural network depth, shallow vs deep networks, function approximation, synthetic data, ReLU networks, MSE evaluation, parameter efficiency, PyTorch, regression
