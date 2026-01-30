# KNN – Handwritten Digit Classification

## Project Overview
This project implements a **K-Nearest Neighbors (KNN)** classifier to recognize handwritten digits using the **Sklearn Digits dataset**. A manual KNN approach using distance computation was applied to classify digits based on similarity.

---

## Dataset Details
- Source: `sklearn.datasets.load_digits()`
- Total Samples: **1797**
- Features: **64 (8×8 pixel images)**
- Classes: **Digits 0–9**

**Dataset Shape:**
- X shape: `(1797, 64)`
- y shape: `(1797,)`

---

## Tools & Libraries Used
- Python  
- NumPy  
- SciPy  
- Scikit-learn  
- Matplotlib  

---

## Methodology
1. Loaded digits dataset and verified feature & label shapes
2. Visualized sample handwritten digit images
3. Split dataset into **80% training** and **20% testing**
4. Applied **StandardScaler** for feature normalization
5. Implemented **manual KNN** using distance calculation (`cdist`)
6. Evaluated accuracy using **K = 3**
7. Tested multiple K values (**3, 5, 7, 9**)
8. Plotted **Accuracy vs K graph**
9. Generated **Confusion Matrix**
10. Displayed test images with **True vs Predicted labels**

---

## Results

### Accuracy for Different K Values
| K Value | Accuracy |
|--------|----------|
| 3 | 0.9694 |
| 5 | 0.9750 |
| 7 | 0.9722 |
| 9 | 0.9722 |

**Best K:** `5`  
**Highest Accuracy:** **97.5%**

---

## Visual Outputs
- **Accuracy vs K plot** to identify best K
- **Confusion Matrix** to analyze classification errors
- **Sample Predictions** showing True vs Predicted digit labels

---

## Conclusion
The KNN model achieved **approximately 97% accuracy**, demonstrating strong performance in handwritten digit classification. Minor misclassifications occurred mainly between visually similar digits, but overall the model performed effectively.

