# 🔢 Full-Fledged Multiple Linear Regression Project  

This project applies **Multiple Linear Regression (MLR)** on a **real-world dataset** from Kaggle.  
We worked with two features and one target variable, trained the model, visualized it in 3D, and also compared results from **Scikit-Learn** and a **custom MLR implementation (coded from scratch)**.  

📂 Dataset Link: [Multiple Linear Regression Dataset](https://www.kaggle.com/datasets/hussainnasirkhan/multiple-linear-regression-dataset)  

---

## 🚀 Project Steps  

### 1. Importing Libraries  
- **NumPy, Pandas** → Data handling  
- **Matplotlib, Seaborn** → Data visualization  
- **Plotly Express & Graph Objects** → 3D visualization of features and hyperplane  
- **Sklearn (train_test_split, LinearRegression, r2_score)** → Model building and evaluation  
- **os, kagglehub** → Dataset access  

### 2. Loading the Dataset  
- Loaded dataset into a Pandas DataFrame.  
- Checked for **null values and duplicates** → None found.  

### 3. Data Visualization  
- **3D Scatter Plot** → Showed relation of both features with the target.  
- **Individual Scatter Plots** → Plotted each feature against the target separately to see how strongly they correlate.  

### 4. Splitting the Data  
- Separated into **X (features)** and **y (target)**.  
- Applied **train-test split (80:20, random_state=2)**.  

### 5. Training with Scikit-Learn  
- Created a **LinearRegression** object.  
- Fitted the model on training data and predicted on test data.  
- Results:  
  - **R² Score:** `0.95`  
  - **Coefficients:** `[-102.88, 2191.86]`  
  - **Intercept:** Found automatically  

### 6. Training with Custom MLR (From Scratch)  
- Used a custom MLR class (written separately and detailed in another repository).  
- Implemented with **Normal Equation**:  
  \[
  \beta = (X^T X)^{-1} X^T y
  \]  
- Custom model gave **exact same results** as Scikit-Learn (R² and coefficients).  
- ✅ This validated that our implementation works correctly.  

### 7. Hyperplane Visualization  
- Plotted the **resulting regression hyperplane** in 3D along with data points.  
- Helped in visualizing how well the plane fits the dataset.  

---

## 📈 Results  

- **Scikit-Learn & Custom MLR matched perfectly**  
- **R² Score:** `0.95` → Model explains 95% of the variance in target.  
- **Coefficients:** `[-102.88, 2191.86]`  
- ✅ Model is highly accurate and reliable.  

---

## 🛠️ Tech Stack  

- **Python**  
- **NumPy, Pandas**  
- **Matplotlib, Seaborn**  
- **Plotly**  
- **Scikit-Learn**  

---

## 📌 Conclusion  

This project showed how Multiple Linear Regression can be applied to **real-world data**.  
- Achieved a very high **R² score of 0.95**.  
- Verified that our **custom-coded MLR** matches Scikit-Learn results.  
- Visualized the regression **hyperplane in 3D**, making the concept easier to understand.  

📓 The full code and outputs are available in the **Jupyter Notebook** included in this repository.  

---
