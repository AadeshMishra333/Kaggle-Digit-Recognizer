# Kaggle-Digit-Recognizer
Week 2 Mini Competition 1 - Classification problem from Kaggle Challenge set

# 🧮 Digit Recognizer — Micro ML Project

**A beginner-friendly image classification project using the Kaggle “Digit Recognizer” (MNIST) dataset.**

---

## 📘 Overview
This competition predicts handwritten digits (0–9) from grayscale images using the MNIST dataset — the “hello world” of computer vision.  
A perfect starting point to explore basic image processing and classical ML models before moving to deep learning.

---

## 🧠 Dataset
**Source:** Kaggle — [Digit Recognizer Competition](https://www.kaggle.com/c/digit-recognizer)

The dataset contains 28×28 grayscale images (784 pixels total). Each pixel value ranges from **0 (white)** to **255 (black)**.

### Files Used
- `train.csv` — 785 columns (first column = label, remaining 784 = pixel values)
- `test.csv` — same as training set but without the label column

Each pixel column (e.g., `pixelx`) represents a specific location in the 28×28 image grid, where  
`x = i * 28 + j` → `i` = row, `j` = column (0-based indexing).

Example:
```
000 001 002 003 ... 026 027
028 029 030 031 ... 054 055
...
756 757 758 759 ... 782 783
```

### 📤 Desired Submission
Your output must include predictions for all 28,000 test images:

```
ImageId,Label
1,3
2,7
3,8
...
```

---

## ⚙️ Tools & Libraries
- Python  
- Jupyter Notebook  
- Pandas, NumPy  
- Scikit-learn  
- Seaborn, Matplotlib

---

## 🚀 Workflow
### 1. Data Preprocessing
- Dataset is already clean — split into training and validation sets.

### 2. Model Training
Trained and compared **classical ML models**:
- **SVM:** Highest accuracy, slower training  
- **Random Forest:** Balanced speed and performance  
- **KNN:** Extremely fast  

**Model Accuracies:**
| Model | Accuracy (%) |
|--------|---------------|
| SVM | 97.27 |
| Random Forest | 96.20 |
| KNN | 96.51 |

### 3. Model Selection
Selected the most accurate and efficient model for final predictions.

### 4. Submission
Generated predictions for `test.csv` and submitted results to Kaggle.

---

## 📊 Results
- **Kaggle Submissions:**  
  - **KNN:** 0.96378 accuracy  
  - **SVM:** 0.9732 accuracy  
- **Best Rank:** 🏆 *674 / 944 participants*

---

## 💡 Learnings
- Basics of Computer Vision and feature representation  
- Classical ML models for classification (KNN, Random Forest, SVM)  
- Evaluating models using Confusion Matrix and accuracy metrics  
- Building a complete pipeline for Kaggle competitions  
- Understanding performance–speed tradeoffs among models
