# **Project 1: Prediction of Treatment Response in Breast Cancer Patients**

## **Description**
This project addresses the prediction of neoadjuvant treatment response in breast cancer patients through the integration of multi-omics data and advanced Machine Learning algorithms. It combines clinical, transcriptomic, immune system, and digital pathology data to develop a robust model that facilitates clinical decision-making and therapy personalization.

---

## **Objectives**
1. Analyze multi-omics data to identify relevant variables associated with treatment response.
2. Develop and evaluate predictive models (Random Forest, Neural Networks, GLM).
3. Compare performance metrics across individual and combined datasets.
4. Select the most important variables through recursive feature elimination and biological interpretation.

---

## **Techniques and Libraries**
- **Exploratory Analysis and Visualization**: `dplyr`, `tidyr`, `ggplot2`, `corrplot`, `ggcorrplot`.
- **Predictive Modeling**:  
  - Random Forest: `caret`, `ranger`.  
  - Neural Networks: `keras`, `tensorflow`, `mlbench`.  
  - GLM and Model Optimization: `stats`, `lattice`, `caret`.  
- **Parallelization and Performance**: `parallel`, `doParallel`.  
- **Evaluation Metrics**: ROC curves (`pROC`), accuracy, sensitivity, specificity, and kappa.

---

## **Methodology**
### **Exploratory Analysis**
- Identification of relationships between variables using correlation matrices.
- Visualization of distributions and detection of outliers.

### **Predictive Models**
- Implementation of Random Forest, Neural Networks, and GLM algorithms.
- Hyperparameter optimization via cross-validation.

### **Data Fusion**
- Integration of clinical, transcriptomic, immune system, and digital pathology datasets.
- Recursive elimination of redundant variables to reduce noise and improve precision.

### **Biological Interpretation**
- Analysis of key variables such as ESR1, PGR, lymphocyte density, and Allred score.
- Evaluation of their impact on cancer progression and treatment response.

---

## **Results**
### **Optimal Model (Random Forest)**
- **Accuracy**: 89.29%.  
- **Sensitivity**: 57.14%.  
- **Specificity**: 100%.  
- **Kappa Value**: 0.6667 (substantial agreement).

### **Model Comparison**
- The combined dataset model outperformed individual datasets across key metrics.
- Neural Networks showed good performance but lower specificity (80%) compared to Random Forest.

### **Key Variables**
- **ESR1 and PGR**: Hormonal receptors.  
- **Lymphocyte Density**: Immune system indicator.  
- **Principal Components**: Derived from RNA-seq gene expression data.

---

## **Conclusion**
The integration of multi-omics data significantly improves the predictive capacity of the model. Recursive feature elimination techniques identify critical features that are valuable for designing personalized therapies. This approach demonstrates the potential of Machine Learning in supporting clinical decisions and advancing cancer treatment strategies.

---

## **Visualizations**
- **ggplot2-generated plots** for model metrics and variable importance.  
- **ROC curves** comparing the performance of predictive models.

---

## **Repository Structure**
- **`Scripts/`**: Contains the R script `Proyecto_ML.Rmd` used for data processing and modeling.
- The data is derived from the study outlined in the paper ["Multi-omic machine learning predictor of breast cancer therapy response"](https://doi.org/10.1038/s41586-021-04278-5) and from the GitHub repository [cclab-brca/neoadjuvant-therapy-response-predictor](https://github.com/cclab-brca/neoadjuvant-therapy-response-predictor).

---

## **How to Reproduce**
1. Clone this repository:
   ```bash
   git clone https://github.com/anam16/Projects-Data-Analyst.git
   cd Projects-Data-Analyst/Project-1-Prediction-ML/
   ```
2. Install the necessary R libraries mentioned in `analysis.R`.
3. Run the analysis script:
   ```R
   source("Scripts/analysis.R")
