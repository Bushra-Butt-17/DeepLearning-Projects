
---

# 🐱 Logistic Regression with a Neural Network: Cat Classification from Scratch 🤖

## 🚀 Project Overview
In this project, we implement **Logistic Regression using a Neural Network** from scratch to classify images of cats and non-cats. The neural network is designed using basic concepts of forward propagation, backpropagation, and optimization, without relying on libraries like TensorFlow. This simple yet powerful approach allows us to understand the inner workings of a neural network while applying it to the task of image classification.

## 🗂 Repository Structure

The repository follows a clear directory structure:

```
Logistic-Regression-with-Neural-Network/
├── datasets/
│   │   └── ...
└── Logistic_Regression_with_Neural_Network.ipynb  # Main notebook

```

- **`datasets/`**: Contains images of cats and non-cats used for training and testing.
- **`Logistic_Regression_with_Neural_Network.ipynb`**: The Jupyter notebook containing all the code, data preprocessing, and model training steps.

## 🛠️ Requirements

To run this project, you need the following Python libraries:

- `numpy`
- `matplotlib`
- `PIL` (for image loading and processing)
- `scikit-learn` (for evaluation metrics like confusion matrix)



## 🧠 Model Architecture

This neural network for logistic regression is implemented from scratch using the following steps:

1. **Data Preprocessing**: Convert the images into a format suitable for training the network (flattening images into vectors and normalizing pixel values).
2. **Forward Propagation**: Compute the output using the current weights and biases of the network.
3. **Backpropagation**: Update the weights and biases based on the error (using gradient descent).
4. **Training**: Use a loop to iteratively train the model and optimize the parameters.

### Model Code Example:

```python
import numpy as np

# Initialize weights and bias
weights = np.zeros((num_features, 1))
bias = 0

# Forward propagation function (sigmoid activation)
def sigmoid(z):
    return 1 / (1 + np.exp(-z))

# Compute the loss function (binary cross-entropy)
def compute_loss(y_true, y_pred):
    m = len(y_true)
    loss = -(1/m) * np.sum(y_true * np.log(y_pred) + (1 - y_true) * np.log(1 - y_pred))
    return loss

# Backpropagation function (gradient descent)
def backpropagation(X, y, y_pred, learning_rate):
    m = len(y)
    dw = (1/m) * np.dot(X.T, (y_pred - y))
    db = (1/m) * np.sum(y_pred - y)
    
    # Update weights and bias
    weights -= learning_rate * dw
    bias -= learning_rate * db

    return weights, bias
```

## 🏋️‍♀️ Training the Model

Train the model on the **cats and non-cats** dataset by iterating through the training data, performing forward and backward propagation at each step. The model parameters (weights and biases) are updated using gradient descent.

```python
for epoch in range(epochs):
    # Forward propagation
    y_pred = sigmoid(np.dot(X_train, weights) + bias)
    
    # Compute loss
    loss = compute_loss(y_train, y_pred)
    
    # Backpropagation
    weights, bias = backpropagation(X_train, y_train, y_pred, learning_rate)
    
    if epoch % 100 == 0:
        print(f"Epoch {epoch}: Loss = {loss}")
```

## 📈 Results and Evaluation

After training the model, you can evaluate its performance using **accuracy**, **precision**, and **recall**. The following metrics are calculated:

- **Confusion Matrix**: Shows the number of true positives, true negatives, false positives, and false negatives.

```python
from sklearn.metrics import confusion_matrix
import seaborn as sns
import matplotlib.pyplot as plt

# Predict using the trained model
y_pred = sigmoid(np.dot(X_test, weights) + bias)
y_pred_label = (y_pred >= 0.5).astype(int)

cm = confusion_matrix(y_test, y_pred_label)

sns.heatmap(cm, annot=True, fmt='d', cmap='Blues', xticklabels=['Non-Cat', 'Cat'], yticklabels=['Non-Cat', 'Cat'])
plt.title('Confusion Matrix')
plt.show()
```

## 📄 Conclusion

This project provides an end-to-end implementation of **Logistic Regression using a Neural Network**, built from scratch, to classify images of cats and non-cats. The steps include:

- Loading and preprocessing the dataset.
- Implementing forward and backward propagation manually.
- Training the model and evaluating the results.
- Evaluating performance using accuracy, loss, and confusion matrix.

By the end of this project, you will have a deeper understanding of how neural networks work and how logistic regression can be applied for binary image classification.

## 📄 License

This project is licensed under the MIT License. See the `LICENSE` file for more details.

---

