# AI Coursework Project — Customer Total Charges Prediction

This repository contains my **Artificial Intelligence coursework project**, where I build two predictive AI models — a **Decision Tree Regressor** and an **Artificial Neural Network (ANN)** — to estimate **Total Charges** for telecom customers.  

The project follows the exact workflow and coding style used in class, including preprocessing steps, leakage-free transformations, train-test splitting, and evaluation using **R² score**.

---

## 📌 Coursework Goals

The aim of this AI coursework project is to:

- Understand the flow of an AI pipeline  
- Apply proper data preprocessing used in AI/ML  
- Handle missing values without causing data leakage  
- Apply categorical encoding (One-Hot Encoding)  
- Use scaling correctly based on training data  
- Implement two AI-based models:
  - **Decision Tree (symbolic AI technique)**
  - **Artificial Neural Network (connectionist AI technique)**  
- Compare and evaluate both models using R²  
- Produce visualisations of predictions  

---

## 📂 Project Structure (based on class workflow)

### **Task 1 — Data Loading & Exploration**
- Loaded dataset using pandas  
- Assigned correct column names  
- Displayed first rows, shape, dtypes  
- Identified missing values  
- Dropped irrelevant ID column  

---

### **Task 2 — Preprocessing (AI Pipeline)**
#### ✔ Missing Value Handling (leakage-preventing)
- Computed:
  - `train_means` for numeric features  
  - `train_modes` for categorical features  
- Filled training data using these values  
- Applied the **same fill values** to the test set  
- Handled missing values in the target `totalCharges`

*(Matching the approach taught in class: fit only on training, transform both.)*

#### ✔ Feature Engineering
- One-hot encoded:
  - `streaming`, `contract`, `payMethod`, `churn`
- Dropped original categorical columns  
- Scaled numeric features (`tenure`, `monthlyCharges`) using **training-based Z-score scaling**  

---

### **Task 3 — Decision Tree Regression (Symbolic AI)**
- Trained a `DecisionTreeRegressor` on preprocessed training data  
- Predicted on test set  
- Evaluated using **R² Score**  
- Visualised Actual vs Predicted values  

---

### **Task 4 — Artificial Neural Network (Connectionist AI)**
Built a fully-connected ANN using Keras:


**Reasoning (as required in coursework):**
- Hidden layers with **ReLU** activation help capture non-linear behavior  
- 8 neurons balance performance and avoid overfitting  
- Linear output is required for regression  
- Adam optimizer provides stable gradient updates  

Trained for **1000 epochs** with validation on test data.

---

### **Task 5 — Model Evaluation**
- Evaluated ANN and Decision Tree using R²  
- ANN expected to outperform the Decision Tree  
- Compared results  
- Generated prediction scatter plot  

---

## 🧪 AI Techniques Demonstrated

- Supervised learning  
- Symbolic AI (Decision Trees)  
- Connectionist AI (Neural Networks)  
- Feature scaling & encoding  
- AI pipeline design  
- Avoiding data leakage  
- Model comparison using R²  

---

## 📦 Technologies & Libraries

- Python
- NumPy
- Pandas
- Scikit-Learn  
- TensorFlow / Keras  
- Matplotlib  

---

## 📈 Results Summary

The ANN produced a higher R² score than the Decision Tree, showing better generalisation ability — matching expected AI behaviour discussed in class.

---

## 📝 Coursework Submitted By

**Yarushah E. Sardar**  
*BSc Computer Engineering — Artificial Intelligence Coursework*

---

## 📧 Contact

If you'd like this README expanded into a report-style PDF for submission, feel free to ask.
