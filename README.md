# 🌀 KNN U-Shape Classification Project

## 📘 Overview
This project demonstrates the implementation of the **K-Nearest Neighbors (KNN)** algorithm using a **U-Shape dataset**. The main objective is to classify data points into two classes and visualize the **decision boundary** of the trained model.

## 📂 Dataset
The dataset used is **ushape.csv** which contains two features (X, Y) and one target variable (class). It forms a U-shaped distribution, ideal for demonstrating how KNN handles non-linear patterns.

### Example of the dataset:
| X | Y | class |
|---|---|--------|
| 0.03 | 0.98 | 0 |
| 0.25 | 0.85 | 1 |
| 0.12 | 0.64 | 0 |

## ⚙️ Project Workflow
1️⃣ **Import Libraries**  
Libraries like pandas, numpy, matplotlib, sklearn, and mlxtend were used for data manipulation, model building, and visualization.

2️⃣ **Load and Rename Columns**  
The dataset was loaded using pandas and columns were renamed for clarity:  
`X`, `Y`, and `class`.

3️⃣ **Data Visualization**  
The dataset was plotted using scatter plot with color mapping by class to show the U-shape data distribution.

4️⃣ **Data Splitting and Scaling**  
The dataset was split into 70% training and 30% testing using train_test_split. StandardScaler was used for normalization to ensure uniform feature scaling.

5️⃣ **Model Training using KNN**  
Multiple K values (1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 20, 50) were tested using 10-fold cross-validation to determine the best K value. The best K was chosen based on the highest cross-validation accuracy score.

6️⃣ **Best K Value Selection**  
The optimal K value was identified and used to train the final KNN model.

7️⃣ **Decision Boundary Visualization**  
Using mlxtend’s plot_decision_regions, the decision boundary for the best K value was plotted, showing clear classification regions of the two classes.

8️⃣ **Model Evaluation**  
The trained model was evaluated on the test set using multiple metrics including Accuracy, Precision, Recall, F1 Score, and AUC-ROC.

## 📊 Results Summary
| Metric | Description | Result |
|---------|--------------|--------|
| **Accuracy** | Overall model correctness | High |
| **Precision** | Correct positive predictions | Good |
| **Recall** | True positive rate | Balanced |
| **F1 Score** | Balance between precision & recall | Strong |
| **AUC-ROC** | Class separability | Excellent |

✅ The KNN model effectively captured the **non-linear decision boundary** of the U-shaped data and provided high accuracy and generalization.

## 🧠 Key Learnings
- KNN performs effectively for **non-linear datasets** like U-shape.  
- **Cross-validation** helps determine the most optimal K value.  
- **Decision boundary visualization** gives clear insight into model behavior.

## 💻 Technologies Used
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Scikit-learn  
- mlxtend

## 📈 Example Output
Best K Value: 3  
Accuracy: 0.95  
Precision: 0.93  
Recall: 0.94  
F1 Score: 0.94  
AUC-ROC: 0.97  

## 🚀 How to Run the Project
1. Clone this repository  
   `git clone https://github.com/yourusername/KNN-UShape-Classification.git`  
2. Open the project in Google Colab or Jupyter Notebook.  
3. Run all the cells sequentially.  
4. Observe the accuracy metrics and the decision boundary visualization.

## 🧑‍💻 Author
**Shaik Shabana**  
📍 Data Science Intern | Python & Machine Learning Enthusiast  
🔗 [GitHub Profile](https://github.com/shaik-shabana05/KNN-Project/blob/main/S_KNN_project.ipynb)


