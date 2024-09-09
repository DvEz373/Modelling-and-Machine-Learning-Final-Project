# Final Project: Classification of Polluted Silicone Rubber Insulators using Machine Learning

## Overview

This project focuses on using machine learning (ML) techniques to classify silicone rubber (SR) insulators contaminated with various pollutants. The project utilizes Laser-Induced Breakdown Spectroscopy (LIBS) data to identify pollutants and employs various ML models to enhance classification accuracy.

### Key Objectives:
- Perform elemental analysis of polluted SR insulators using LIBS.
- Classify the contaminated SR samples using machine learning algorithms.
- Compare the performance of different ML models to identify the most accurate and efficient classifier.

---

## Dataset

The dataset used for this project consists of spectral data captured from LIBS analysis of silicone rubber insulators coated with seven different types of artificially prepared pollutants. 

- **Number of Samples:** 1400 (200 samples per pollutant type)
- **Number of Features:** 2048 spectral data points per sample
- **Pollutant Types:**
  1. NaCl
  2. CuSO₄
  3. Fly ash
  4. Coal
  5. Cement
  6. Ca₃(PO₄)₂ (Fertilizer)
  7. Combination of all

---

## Machine Learning Models

The following machine learning algorithms were used for classification:

1. **Linear Discriminant Analysis (LDA)**  
   - Training Accuracy: 100%  
   - Testing Accuracy: 74.29%  
   - Overall Accuracy: 94.86%  
   - Execution Time: 2.2s  

2. **Decision Tree**  
   - Training Accuracy: 100%  
   - Testing Accuracy: 74.29%  
   - Overall Accuracy: 94.86%  
   - Execution Time: 4.0s  

3. **K-Nearest Neighbors (KNN)**  
   - Training Accuracy: 100%  
   - Testing Accuracy: 80.71%  
   - Overall Accuracy: 96.14%  
   - Execution Time: 0.6s  

4. **Gradient Boosting**  
   - Training Accuracy: 100%  
   - Testing Accuracy: 82.14%  
   - Overall Accuracy: 96.43%  
   - Execution Time: 581.6s  

5. **Histogram-Based Gradient Boosting**  
   - Training Accuracy: 100%  
   - Testing Accuracy: 85.00%  
   - Overall Accuracy: 97.00%  
   - Execution Time: 174.7s  

6. **Extreme Gradient Boosting (XGBoost)**  
   - Training Accuracy: 100%  
   - Testing Accuracy: 84.64%  
   - Overall Accuracy: 96.92%  
   - Execution Time: 29.6s  

7. **Light Gradient Boosting (LightGBM)**  
   - Training Accuracy: 100%  
   - Testing Accuracy: 87.14%  
   - Overall Accuracy: 97.43%  
   - Execution Time: 5.1s

---

## Results

The **Light Gradient Boosting** algorithm achieved the highest classification accuracy of 97.43% while maintaining a reasonable execution time of 5.1 seconds. This technique proves to be the best model for this classification task, combining high accuracy with efficient computation.

---

## How to Run

1. Clone this repository.
2. Install the required Python packages by running:

   ```bash
   pip install -r requirements.txt
   ```

3. Run the Jupyter notebook for training and evaluating the models:

   ```bash
   jupyter notebook TugasBesar_1.ipynb
   ```

4. Load the dataset (`dataset_2.csv`) and execute the notebook cells to reproduce the results.

These are the core libraries for:

- **NumPy and pandas**: Data manipulation and array handling.
- **Scikit-learn**: General machine learning models (LDA, Decision Tree, KNN, Gradient Boosting).
- **LightGBM and XGBoost**: Gradient boosting algorithms.
- **Matplotlib and Seaborn**: Data visualization.
- **Jupyter**: Running the notebook environment.

## Conclusion

This project demonstrates the power of machine learning in classifying complex spectral data derived from LIBS analysis. The use of advanced gradient boosting techniques like LightGBM led to optimal classification performance, making it a valuable tool for pollution identification in industrial applications.