# 🍷 Wine Quality Prediction using Machine Learning

## 🌟 Project Overview
This project predicts the **quality of wine** based on its physicochemical properties using machine learning. Wine quality is rated on a scale from 0 to 10 and depends on chemical features such as acidity, sugar content, pH, alcohol, and sulfur levels.  

The model classifies wines as **Good 🍇** (quality ≥ 7) or **Bad ❌** (quality < 7) using a **Random Forest Classifier**. This demonstrates how ML can uncover hidden patterns in wine chemistry to help winemakers optimize production and assist consumers in making informed choices.

---

## 📊 Dataset
- **Source:** [UCI Wine Quality Dataset](https://archive.ics.uci.edu/ml/datasets/wine+quality)  
- **Type:** Red wine dataset  
- **Number of features:** 11 physicochemical attributes  
- **Target:** Wine quality (0–10)  

### 🍾 Features
| Feature | Description |
|---------|-------------|
| Fixed acidity | Amount of fixed acids |
| Volatile acidity | Amount of acetic acid |
| Citric acid | Amount of citric acid |
| Residual sugar | Sugar left after fermentation |
| Chlorides | Amount of salt |
| Free sulfur dioxide | Free SO₂ in wine |
| Total sulfur dioxide | Total SO₂ in wine |
| Density | Wine density |
| pH | Acidity level |
| Sulphates | Sulfate content |
| Alcohol | Alcohol percentage |

---

## 🔎 Exploratory Data Analysis
- Checked distributions of wine quality scores and features  
- Visualized relationships between features (e.g., alcohol, citric acid, volatile acidity) and wine quality  
- Performed correlation analysis to identify features strongly affecting quality  
- Heatmap visualization to understand feature interactions  

**Observations:**  
- 🍸 Alcohol and citric acid positively correlate with quality  
- ⚠️ Volatile acidity negatively correlates with quality  
- Sulphates, density, and pH also influence wine quality  

---

## 🌳 Machine Learning Model
**Random Forest Classifier** was used to predict wine quality.  

**Why Random Forest?**  
- Ensemble method combining multiple decision trees  
- Reduces overfitting compared to a single tree  
- Captures complex, non-linear relationships  
- Provides feature importance to identify influential features  

**Advantages in this project:**  
- Handles high-dimensional data effectively  
- Performs well for binary classification (Good 🍇 vs Bad ❌)  
- Generalizes well to unseen data  

---

## 🏷️ Label Binarization
Wine quality was converted into binary labels for classification:  
- **Good wine 🍇:** quality ≥ 7 → Label `1`  
- **Bad wine ❌:** quality < 7 → Label `0`  

This simplifies the task and focuses on identifying high-quality wines.

---

## 📈 Model Training & Evaluation
The Random Forest model was trained on the dataset and evaluated on unseen test data.  

### Performance Metrics:
- **Training Accuracy:** 100% ✅  
- **Test Accuracy:** 92.81% 🎯  

**Additional Evaluation:**  
- Confusion Matrix: correctly predicts both good and bad wines  
- Classification Report: high precision, recall, and F1-score for both classes  
- Feature Importance: alcohol, sulphates, and citric acid were the most influential  

**Conclusion:**  
The model demonstrates excellent predictive ability and reliability for wine quality classification. 🍷

---

## 🚀 Usage
Users can input physicochemical properties of a wine sample to get a prediction:  
- **Good Wine 🍇**  
- **Bad Wine ❌**  

It can be used interactively or to batch process multiple wine samples.

---

