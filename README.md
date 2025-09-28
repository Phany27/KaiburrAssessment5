
# Kaiburr Task 5 - Text Classification Assessment

This repository contains the solution for **Kaiburr Task 5**, where we perform **text classification on consumer complaints data** using multiple machine learning models. The notebook walks through the complete pipeline: **data preprocessing, exploratory data analysis (EDA), feature extraction, model training, evaluation, and comparison**.

---

## 📌 Project Overview
The goal of this assessment is to classify **consumer complaint narratives** into predefined categories:
- **Credit reporting, repair, or other**
- **Debt collection**
- **Consumer Loan**
- **Mortgage**

We build and evaluate several models to identify the best-performing classifier.

---

## 🛠️ Tech Stack
- **Python**
- **Libraries**:
  - Data handling: `pandas`, `numpy`
  - Text preprocessing: `nltk`, `re`
  - Feature engineering: `scikit-learn` (`TfidfVectorizer`, `CountVectorizer`)
  - Models: Logistic Regression, Naive Bayes, Linear SVC, Random Forest
  - Visualization: `matplotlib`, `seaborn`, `wordcloud`

---

## 📂 Repository Structure
---

## 🚀 Steps Performed

### **1. Data Loading**
- Loaded the complaints dataset (`complaints.csv`).
- Selected four major product categories for classification.
- Cleaned data by handling **missing values** and removing **duplicates**.

---

### **2. Text Preprocessing**
- Converted text to lowercase.
- Removed **special characters, digits, and extra spaces**.
- Tokenized words and removed **stopwords**.
- Applied **lemmatization** using NLTK.

**Function implemented:** `preprocess_text(text)`

---

### **3. Exploratory Data Analysis (EDA)**
- **Category distribution** visualization using bar plots.
- **Text length analysis** (average complaint length per category).
- **Boxplots** to understand text length variability.
- **Histograms** for distribution of complaint lengths.
- **Top n-grams** extracted for each category.

---

### **4. Train-Test Split**
- Split the dataset into **75% training** and **25% testing**.
- Applied **stratified sampling** to preserve class balance.

---

### **5. Model Training & Evaluation**
We trained multiple models with a **TF-IDF feature representation**:

#### 🔹 Logistic Regression
- Solver: `liblinear`
- Multi-class strategy: One-vs-Rest

#### 🔹 Naive Bayes (MultinomialNB)
- Simple probabilistic model for text classification.

#### 🔹 Linear SVC
- Linear Support Vector Machine for high-dimensional text data.

---

### **6. Performance Metrics**
For each model:
- **Accuracy**
- **Confusion Matrix**
- **Classification Report** (Precision, Recall, F1-Score)

---

### **7. Results & Comparison**
- Plotted a **bar chart** comparing model accuracies.
- Observed which algorithm performs best on the complaint classification task.

- https://github.com/Phany27/KaiburrAssessment5/blob/main/Screenshot%202025-09-28%20231912.png
- https://github.com/Phany27/KaiburrAssessment5/blob/main/Screenshot%202025-09-28%20231919.png
- https://github.com/Phany27/KaiburrAssessment5/blob/main/Screenshot%202025-09-28%20231954.png
- https://github.com/Phany27/KaiburrAssessment5/blob/main/Screenshot%202025-09-28%20232003.png



## ⚙️ Installation & Usage
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/Kaiburr_Task5.git
   cd Kaiburr_Task5

