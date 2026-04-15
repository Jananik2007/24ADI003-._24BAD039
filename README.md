## Recommendation Systems using Matrix Factorization (SVD & NMF)

##  Overview
This experiment focuses on building a **Recommendation System** using **Matrix Factorization techniques**:
- **Singular Value Decomposition (SVD)**
- **Non-negative Matrix Factorization (NMF)**

The goal is to predict missing user ratings and recommend relevant items (movies).

##  Dataset
- **Name:** MovieLens 100K Dataset  
- **Source:** Kaggle  
- **Features Used:**
  - **User ID**  
  - **Movie ID**  
  - **Ratings**  

##  Objectives
- Understand **matrix factorization techniques**  
- Apply **SVD and NMF** for recommendation systems  
- Predict missing ratings  
- Generate **Top-N recommendations**  
- Compare performance of SVD and NMF  

##  Technologies Used
- **Python**  
- **NumPy**  
- **Pandas**  
- **Matplotlib**  
- **Seaborn**  
- **Scikit-learn**  
- **Surprise Library**  

## Scenario 1: Matrix Factorization using SVD

### Description
**SVD (Singular Value Decomposition)** decomposes the user-item matrix into latent factors to capture hidden relationships between users and items.

###  Steps
1. Import required libraries  
2. Load MovieLens dataset  
3. Perform data preprocessing  
4. Create **User-Item Interaction Matrix**  
5. Normalize matrix (optional – mean centering)  
6. Apply **SVD decomposition**  
7. Reduce dimensions (**select k latent factors**)  
8. Reconstruct the matrix  
9. Predict missing ratings  
10. Generate **Top-N recommendations**  

###  Evaluation Metrics
- **RMSE (Root Mean Square Error)**  
- **MAE (Mean Absolute Error)**  

### Visualizations
- Heatmap of **original vs reconstructed matrix**  
- Error vs number of latent factors  
- Top recommended movies  

##  Scenario 2: Matrix Factorization using NMF

###  Description
**NMF (Non-negative Matrix Factorization)** decomposes the matrix into non-negative factors, making it easier to interpret latent features.

###  Steps
1. Load dataset  
2. Create **User-Item matrix**  
3. Handle missing values (fill with 0 or mean)  
4. Apply **NMF model**  
5. Factorize into:
   - User-feature matrix  
   - Item-feature matrix  
6. Reconstruct rating matrix  
7. Predict missing values  
8. Generate **Top-N recommendations**  

### Evaluation Metrics
- **RMSE**  
- **Precision@K**  
- **Recall@K**  

### Visualizations
- Latent feature visualization  
- Reconstruction comparison  
- Recommendation ranking chart  

##  Key Analysis

### SVD
- Captures **latent relationships** effectively  
- Works well with sparse data  
- May produce **negative values**  

### NMF
- Produces **only non-negative values**  
- More **interpretable factors**  
- Useful for recommendation explainability  

##  Results
- Successfully predicted **missing ratings**  
- Generated **Top-N movie recommendations**  
- Observed differences in:
  - Accuracy (**SVD better**)  
  - Interpretability (**NMF better**)  

##  Repository Contents
- Python Code Files  
- Dataset  
- Output Screenshots  
- Graphs and Visualizations  
