# **Task-4: Classification with Logistic Regression**

### **Dataset**

* **File:** `data.csv`
* **Location:** Local upload
* **Target Variable:** `diagnosis`
  * **1:** Malignant (Cancer)
  * **0:** Benign (No Cancer)

### **Tools & Libraries**

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn

### **Steps Performed**

1. **Loaded the dataset**
   * Dropped unnecessary columns like `id` and `Unnamed: 32`.
   * Checked dataset shape, used `head()` and `info()` for initial understanding.
2. **Preprocessed the data**
   * Converted target variable `diagnosis` into binary numeric form (M=1, B=0).
   * Split data into **features (X)** and **target (y)**.
   * Standardized features using **`StandardScaler()`** to bring all variables to a similar scale.
3. **Split into Train-Test sets**
   * Used **80% for training** and **20% for testing** using `train_test_split()`.
4. **Built the Logistic Regression Model**
   * Applied **`LogisticRegression()`** from Scikit-learn.
   * Trained model using `.fit()` on training data.
5. **Predicted and Evaluated Model Performance**
   * Generated predictions on test set.
   * Calculated:
     * **Confusion Matrix**
     * **Precision, Recall, F1-score** (using `classification_report`)
     * **ROC-AUC Score** (using `roc_auc_score`)
6. **Visualized ROC Curve**
   * Plotted **ROC Curve** using `matplotlib` and `roc_curve`.
   * Compared model performance against a **random (no skill) classifier**.
7. **Threshold Tuning**
   * Tested a **custom classification threshold** (example: 0.4) to show how threshold affects performance metrics.
8. **Explained the Sigmoid Function**
   * Demonstrated the mathematical calculation of the **sigmoid output** for a sample test input.
   * Highlighted how logistic regression converts feature values into a probability between 0 and 1.

### **Output**

* **Evaluation Metrics:**
  * Confusion Matrix, Precision, Recall, F1-score, ROC-AUC.
* **ROC Curve:**
  * Visual comparison between true positive rate and false positive rate.
* **Threshold Sensitivity:**
  * Illustrated how changing the threshold alters classification results.
* **Sigmoid Calculation:**
  * Displayed example showing conversion of raw input to probability.
* **Conclusion:**
  * Logistic Regression successfully classified between malignant and benign cases with reasonable accuracy.
  * Model performance can be fine-tuned further by adjusting threshold or using feature selection.
