# 🌲 Forest Cover Type Prediction  

📖 A machine learning project to predict the **forest cover type** (the predominant kind of tree cover) from cartographic variables.  
The dataset is well-known from the UCI repository and Kaggle, and the task is a **multi-class classification problem**.  

---

## 🚀 Features  
- Load and preprocess the Forest Cover dataset  
- Apply classification algorithms (Decision Tree, Random Forest, XGBoost)  
- Perform **Hyperparameter Tuning** to optimize model performance  
- Feature importance analysis for interpretability  
- Evaluate models with multiple metrics  
- Visualize results: feature correlations, confusion matrix, and accuracy comparison  

---

## 📊 Dataset  
- **Source:** UCI Machine Learning Repository / Kaggle  
- **Instances:** 581,012 samples  
- **Features:** 54 cartographic variables  
  - Elevation, Aspect, Slope  
  - Soil types (categorical)  
  - Wilderness areas (categorical)  
- **Target Classes (7 types of forest cover):**  
  1. Spruce/Fir  
  2. Lodgepole Pine  
  3. Ponderosa Pine  
  4. Cottonwood/Willow  
  5. Aspen  
  6. Douglas-fir  
  7. Krummholz  

---

## ⚙️ Getting Started  

### ✅ Prerequisites  
- Python 3.7 or later  
- pip or other package manager  

# 🧠 Models & Hyperparameter Tuning  
  
### 🔹 Random Forest Classifier  
- Tuned parameters: `n_estimators`, `max_depth`, `max_features`, `min_samples_split`  

### 🔹 XGBoost Classifier  
- Tuned parameters: `learning_rate`, `n_estimators`, `max_depth`, `subsample`, `colsample_bytree`  

### ⚙️ Tuning Method  
- **Grid Search** and **Randomized Search** with **Cross-Validation** were applied to find the optimal hyperparameters.  

---

# 📈 Performance  

The models were evaluated using:  
- **Accuracy**  
- **Precision**  
- **Recall**  
- **F1-score**  

✅ **Random Forest (after tuning)** and **XGBoost (after tuning)** achieved the highest accuracy.  

| Model              | Accuracy (Before Tuning) | Accuracy (After Tuning) |
|--------------------|---------------------------|--------------------------|
| Random Forest      | 0.90                      | 0.94                     |
| XGBoost            | 0.91                      | 0.93                     |

---

# 🔍 Example Prediction  

Input Features:  
- Elevation: `3000`  
- Aspect: `45`  
- Slope: `10`  
- Soil_Type: `10`  
- Wilderness_Area: `2`  

**Predicted Cover Type:** `Spruce/Fir` 🌲  
