# 🚀 Introduction to Planar Data Classification with MLP
![image](https://github.com/user-attachments/assets/f3cc71a4-507a-4dc9-bfc5-4492a431dd5c)

---

## 🚀 **Overview of Planar Data Classification**  
Welcome to the **MLP-Planar-Data-Classification** project! This repository demonstrates how a **Multi-Layer Perceptron (MLP)** can be used to classify **planar data**. Planar data is often **non-linearly separable**, meaning that the two classes cannot be divided by a simple straight line. This project showcases the power of neural networks in solving such problems by learning complex decision boundaries.

The main goal is to show how an MLP can be trained using **gradient descent** and how it can progressively improve through iterations. The project also includes **visualizations** that track the model's learning journey, helping you understand the process more clearly.

---

## 🌟 **Features**  
- **Planar Data Classification** using an MLP 🤖: Classifying data points in a 2D plane using a multi-layer perceptron to handle complex decision boundaries.
  
- **Gradient Descent Optimization** 🔄: The model uses gradient descent to optimize weights and minimize the **binary cross-entropy** loss function.

- **Intuitive Visualizations** 📊:  
  Visualize key aspects of the model’s performance with plots stored in the `Visualizations/` directory, such as:
  - **Decision Boundary** 🔵🟠: Shows how the model separates the two classes.
  - **Loss Curve** 📉: Tracks the model's performance over time.
  - **Accuracy Progression** 📈: Monitors the model’s accuracy across epochs.

- **Step-by-Step Implementation** 📝: Follow a clear, guided implementation with detailed comments and explanations in the notebook, making it beginner-friendly and easy to understand.

---

## 📂 **Directory Structure**  
```
MLP-Planar-Data-Classification/
├── MLP-Planar-Data-Classification.ipynb  # Main implementation notebook 📝
├── Visualizations/                       # Directory containing plots and learning visuals 📊
│   ├── decision_boundary.png             # Visualization of the decision boundary 🔵🟠
│   ├── ...
└── README.md                             # Project documentation 📚
```

---

## 🛠️ **How to Use**  
1. **Run the Notebook:**  
   Open the `MLP-Planar-Data-Classification.ipynb` notebook in a Jupyter Notebook or compatible environment (e.g., VS Code). Execute each cell sequentially to build, train, and evaluate the MLP model.

2. **Explore the Visualizations:**  
   After training the model, check the `Visualizations/` directory for the following:
   - **Decision Boundary** 🔵🟠: Shows how well the MLP can separate the two classes in the 2D space.
   - **Loss Curve** 📉: Displays how the loss decreases as the model learns during training.
   - **Accuracy Progression** 📈: Tracks the accuracy improvement over time.

---

## 🧪 **Technical Details**  
- **Activation Function:** Sigmoid 🟢  
  The **sigmoid activation function** is used to map the model’s output to a value between 0 and 1, which is ideal for binary classification tasks.

- **Loss Function:** Binary Cross-Entropy 📉  
  This loss function is used for binary classification and calculates the error between the predicted probabilities and the actual labels.

- **Optimizer:** Gradient Descent 🚴‍♂️  
  **Gradient descent** updates the model's weights and biases by calculating gradients of the loss function, minimizing the error iteratively during training.
  ![sgd_bad](https://github.com/user-attachments/assets/f5e95ff2-b550-4fc2-b700-6c1faa64ea52)
![sgd](https://github.com/user-attachments/assets/eddee2ec-99e6-4faf-b7aa-0bf0df27465a)


- **Evaluation Metrics:** Accuracy & Visualizations 📈  
  The model’s performance is evaluated based on accuracy and visualizations of the decision boundary and loss curve.
<img width="1182" alt="grad_summary" src="https://github.com/user-attachments/assets/792c4cd9-4741-4796-8a9c-e6b15230b34e" />
<img width="1182" alt="classification_kiank" src="https://github.com/user-attachments/assets/7e6853cf-a942-4d95-857c-dab2184b85b8" />

---

## 📷 **Sample Visualizations**  
- **Loss Curve** 📉: Shows the decrease in loss as the model improves during training.
- **Decision Boundary** 🔵🟠: Displays how the model divides the two classes in planar space.
- **Accuracy Progression** 📈: Tracks the model’s accuracy at each epoch.



  ![image](https://github.com/user-attachments/assets/243ea97d-28da-48fb-be94-74b437bdcd34)
![image](https://github.com/user-attachments/assets/21edb3c3-a8f3-4310-8cb8-6905316455f2)
![image](https://github.com/user-attachments/assets/cf3b4c57-5ffb-4103-baff-dca53db1402b)


![image](https://github.com/user-attachments/assets/c55e4e88-95d4-453f-a32c-0d1862c9e1cb)

---

## 🤝 **Contributing**  
Contributions are welcome! If you have suggestions, improvements, or want to report an issue, feel free to fork the repository, create an issue, or submit a pull request.

---

## 📧 **Contact**  
For any questions or feedback, feel free to reach out via email or by opening an issue on GitHub.  

Happy Learning! 🌟
