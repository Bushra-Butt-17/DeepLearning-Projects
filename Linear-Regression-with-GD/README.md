

---

# 🏠 Ames Housing Price Prediction: Linear Regression with Gradient Descent  

This project demonstrates the implementation of **Linear Regression** from scratch using **Gradient Descent** to predict housing prices in Ames, Iowa. The analysis is based on the famous **Ames Housing Dataset**, a well-known dataset in the Data Science and Machine Learning community.

The notebook, `linear-regression-with-gd.ipynb`, walks through the process of building and optimizing a linear regression model while exploring key concepts in machine learning.  

---

## 📁 Repository Structure  

```plaintext  
├── linear-regression-with-gd.ipynb  # Main Jupyter Notebook with all analysis and code  
├── data/  
│   ├── Ames_Housing.csv            # Full dataset  
├── visualizations/  
└── README.md                       # Project documentation (this file)  
```  

---

## 📊 Dataset Description  

The **Ames Housing Dataset** contains 79 features describing various aspects of residential homes in Ames, Iowa. The target variable is `SalePrice`, representing the price of the home in dollars.

For this project:  
- **Dataset Used:** Combined and preprocessed data from `Ames_Housing.csv`.  
- **Target Variable:** `SalePrice`.  

More information about the dataset can be found [here](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/overview).  

---

## ⚙️ Project Workflow  

1. **Data Preprocessing**  
   - Handle missing values  
   - Apply feature scaling using Min-Max normalization  
   - Select features to improve model efficiency  

2. **Linear Regression from Scratch**  
   - Implement the **Gradient Descent Algorithm** for parameter optimization  
   - Loss function: **Mean Squared Error (MSE)**  

3. **Model Evaluation**  
   - Metrics: **R-squared**, **Mean Absolute Error (MAE)**, and **Root Mean Squared Error (RMSE)**  
   - Comparison with sklearn's linear regression for benchmarking  

4. **Visualization**  
   - Plot the learning curve to show convergence of Gradient Descent  
   - Feature importance visualized with bar charts  

---

## 🔑 Key Features  

- **From Scratch Implementation:**  
  No external libraries were used for training the linear regression model.  

- **Gradient Descent Optimization:**  
  Iteratively updates weights using a user-defined learning rate to minimize the cost function.  

- **Interactive Notebook:**  
  Well-documented and visualized analysis with explanations for each step.  

---

## 📈 Results  

- **Training Loss Convergence:**  
  The learning curve demonstrates the reduction in error as the model learns over iterations.  

- **Feature Importance:**  
  Visualized as a bar chart to highlight the most impactful features, such as `OverallQual` and `GrLivArea`.  

- **Evaluation Metrics on Test Set:**  
  - R² Score: 0.85  
  - MAE: $21,000  
  - RMSE: $27,500  

---

## 📂 Included Files  

- **`linear-regression-with-gd.ipynb`**:  
  Contains all the code and detailed explanations for preprocessing, training, and evaluation.  

- **`data/Ames_Housing.csv`**:  
  Combined dataset used for training and testing the model.  

- **`visualizations/learning_curve.png`**:  
  Visualization showing how the model learns over epochs.  

---

## 🛠️ Technologies Used  

- **Python Libraries:**  
  - `NumPy`: For numerical computations  
  - `Pandas`: For data manipulation  
  - `Matplotlib` and `Seaborn`: For data visualization  

- **Jupyter Notebook:** Interactive development environment.  

---

## 🚀 Future Work  

- Implement feature engineering techniques to enhance model performance.  
- Explore advanced optimization methods like Stochastic Gradient Descent (SGD).  
- Incorporate regularization techniques (L1/L2) to prevent overfitting.  

---

## 🙋‍♀️ Author  

Developed by **Bushra Shahbaz**. If you have any questions or suggestions, feel free to reach out:  
📧 Email: bsdsf21m020@pucit.edu.pk  
🌐 GitHub: [Bushra-Butt-17](https://github.com/Bushra-Butt-17)  

---

## 🌟 Acknowledgments  

- Thanks to [Kaggle](https://www.kaggle.com/) for the dataset.  
- Inspired by Andrew Ng's ML course for a deeper understanding of Gradient Descent.  

---

Feel free to copy, modify, and distribute this project. 😊 Happy Learning!  

--- 


