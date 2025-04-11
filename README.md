# 📊 Market Regime Clustering and Analysis

This project performs **market regime detection** using unsupervised clustering techniques, followed by **visualization**, **regime interpretation**, and **transition analysis**. The regimes are detected based on engineered features such as volatility, spread, volume, and returns.

---

## 📁 Dataset

The dataset contains processed market microstructure data and is stored on Google Drive:

🔗 **[Download Dataset Folder](https://drive.google.com/drive/folders/1gFLwPLTE0nUN-MHoOn5u_1yrlbpI3Fst?usp=sharing)**

Please download and extract this before running the notebook.

---

## 📘 Notebook Overview

The notebook (`regime_analysis.ipynb`) includes the following steps:

### 🛠️ 1. Preprocessing
- Scaling features using `StandardScaler`
- Feature selection: volatility, spread, volume, log returns, bid/ask quantities, etc.

### 🧠 2. Clustering Algorithms
- **KMeans Clustering**
- **HDBSCAN Clustering**
- **Gaussian Mixture Models (GMM)**

### 📊 3.Descriptive Evaluation of Market Regimes

### 🌐 4. Dimensionality Reduction
- **UMAP** for 2D visualization of clusters

### 🖼️ 5. Visualization
- Scatter plot colored by cluster labels
- Regime transition heatmap using Seaborn

### 📈 6. Transition Matrix
- Constructed regime transition probability matrix
- Interpreted how often the market switches regimes

### 📉 7. Regime Interpretability
- Averaged key market statistics per regime (volatility, spread, volume, etc.)
- Inferred high-volatility vs. stable periods based on clustering

---

## 🔧 Requirements

Install the following Python libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn hdbscan umap-learn
