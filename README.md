# Particle-Based Wear Prediction using Machine Learning

This repository contains the code, data, and workflows used in my M.Tech thesis research project titled:  
**"Prediction of Particle-Based Wear Using Machine Learning"**.  

The project combines **Discrete Element Method (DEM) simulations** with **machine learning models** to predict wear behavior based on material, process, and geometric properties.  
The workflow includes **feature engineering, regularization-based feature selection, PCA analysis, and supervised ML models** (Linear Regression, Lasso, Ridge, Decision Tree, and GA-optimized ANN).

## 📂 Files Overview  

### Datasets  
- **wear_prediction_full_features.csv** → Original dataset with all 20+ features.  
- **reduced_feature_dataset.csv** → Feature-reduced dataset after applying Regularization (Lasso/Ridge) and PCA.  

### Model Scripts  
- **Linear_Regression.ipynb** → Baseline linear regression model.  
- **Lasso_Ridge.ipynb** → Feature selection and shrinkage methods (L1 & L2).  
- **PCA.ipynb** → Dimensionality reduction and feature grouping.  
- **Decision_Tree.ipynb** → Nonlinear regression model using recursive splits.  
- **GA_ANN.ipynb** → Neural network optimized using Genetic Algorithm.  

### Outputs  
- Graphs, coefficient plots, feature importance visualizations, and performance metrics.  

---

## 🔄 Workflow / Chronology  

1. **Start with datasets**  
   - Use `wear_prediction_full_features.csv` for baseline models.  
   - Apply feature selection (Lasso, Ridge, PCA) → `reduced_feature_dataset.csv`.  

2. **Run baseline model**  
   - Execute `Linear_Regression.py` to understand feature contributions.  

3. **Apply regularization**  
   - Run `Lasso_Ridge.py` to identify significant features and compare datasets.  

4. **Check dimensionality reduction**  
   - Run `PCA.py` to validate feature groupings and redundancy.  

5. **Train nonlinear model**  
   - Run `Decision_Tree.py` to capture nonlinear interactions.  

6. **Optimize complex model**  
   - Run `GA_ANN.py` to optimize neural networks with Genetic Algorithm.  

7. **Compare performance**  
   - Collect R², MAE, and residual plots from outputs for all models.  

---

## ⚙️ How to Use  

1. **Install dependencies:**  
   ```bash
   pip install -r requirements.txt
