# Day_34_AM
# SVM & KNN - Handwritten Digit Classifier (MNIST Digits)

**Day 33 | AM Session | Week 6**  
**PG Diploma in AI-ML & Agentic AI Engineering | IIT Gandhinagar**

## 📋 Assignment Overview
Take-home assignment focused on **Maximum Margin Classifier, SVM (hard/soft margin, C, gamma, kernel trick)** and **KNN (distance metrics, optimal K, curse of dimensionality)** using the classic MNIST digits dataset (`sklearn.datasets.load_digits`).

## ✅ Tasks Completed

### Part A: Concept Application (40%)
- Loaded `load_digits` dataset
- Applied `StandardScaler` on features
- Trained **SVM with RBF kernel** using `GridSearchCV` on `C` and `gamma`
- Trained **KNN** with optimal `K`
- Compared:
  - Accuracy
  - Confusion matrices
  - Per-class F1 scores
- Identified most commonly confused digits

**Results (as per expected deliverables):**
- **SVM (RBF, C=10, gamma=0.001)** → Accuracy = **0.98**
- **KNN (K=3)** → Accuracy = **0.97**
- Most confused digit pairs: **(3,8), (4,9), (1,7)**

### Part B: Stretch Problem (30%) — FAISS
- Researched **FAISS** (Facebook AI Similarity Search)
- Installed `faiss-cpu`
- Implemented Approximate Nearest Neighbors KNN search on digits dataset
- Compared query speed: `sklearn.KNeighborsClassifier` vs **FAISS** for 1000 queries
- Documented performance findings

### Part C: Interview Ready (20%)
- Answered conceptual question (SVM vs Logistic Regression)
- Implemented `knn_from_scratch()` using only NumPy (Euclidean distance)
- Debugged low-accuracy SVM issue (identified missing feature scaling)

### Part D: AI-Augmented Task (10%)
- Generated interactive Matplotlib visualization showing SVM decision boundary change with `C` (0.01 → 100)
- Used AI to create analogy for **Kernel Trick** and evaluated its accuracy/helpfulness

## 📁 Files
- `svm_knn_digits.ipynb` → Main Jupyter Notebook
- `requirements.txt`
- `README.md` (this file)

# Day_34_PM

---


```markdown
# SVM, KNN & Full Week ML Algorithm Comparison

**Day 33 | PM Session | Week 6**  
**PG Diploma in AI-ML & Agentic AI Engineering | IIT Gandhinagar**

## 📋 Assignment Overview
Take-home assignment to build a **comprehensive ML cheat sheet** for all 8 algorithms learned in Week 6 and perform text classification using **SVM + TF-IDF**.

## ✅ Tasks Completed

### Part A: Concept Application (40%)
- Created an **8-algorithm comparison notebook** (cheat sheet)
- Each algorithm card includes:
  - When to use
  - Key hyperparameters
  - Pros & Cons
  - 5-line code snippet
- Tested **all 8 algorithms** on one dataset with proper cross-validation
- Ranked models and gave final recommendation with reasoning

**Example Card Format:**
```markdown
=== XGBoost ===
When: Tabular data, need best accuracy
Params: n_estimators, learning_rate, max_depth
Pros: Fast, handles missing values, regularized
Cons: Less interpretable

Part B: Stretch Problem (30%) — SVM for Text Classification

Loaded 20newsgroups dataset (4 categories)
Built TF-IDF + LinearSVC pipeline
Trained and evaluated SVM model
Compared performance with Logistic Regression on the same text data

Part C: Interview Ready (20%)

Answered high-dimensional data question (100 features, 50 samples)
Implemented model_selection_report() function with scaling + CV + statistical best model (paired t-test)
Diagnosed SVM overfitting case (train acc 1.0, test acc 0.52) and proposed 3 specific fixes

Part D: AI-Augmented Task (10%)

Used AI to generate a "Decision Tree for Algorithm Selection" based on dataset characteristics
Verified every recommendation against practical experience
Identified edge cases and improved the guide
Saved as personal algorithm selection reference
