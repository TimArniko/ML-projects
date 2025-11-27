# Machine Learning Projects Repository

This repository contains multiple machine-learning projects created as part of coursework and independent study.  
The projects cover supervised and unsupervised learning techniques, including text classification, regression, dimensionality reduction, and representation learning.

---

## 📂 1. Kaggle Projects

### 📰 BBC News Classification  
**Notebook:** `BBC News Classification.ipynb`  
**Datasets:**  
- `BBC News Train.csv`  
- `BBC News Test.csv`  
- `BBC News Sample Solution.csv`

**Summary:**  
This project applies several machine-learning methods to classify BBC News articles into categories.  
It includes:

- Exploratory Data Analysis (EDA)  
- Data preprocessing and duplicate removal  
- TF-IDF vectorization  
- Topic modeling (NMF)  
- Supervised classification using LinearSVC  
- Training-size comparison  
- Kaggle-style prediction file generation  

---

## 📂 2. Supervised Learning

### 📈 Polynomial Regression Analysis  
**Notebook:** `ML-demo1.ipynb`  
**Dataset:** `Messreihe_demo1.csv`

**Summary:**  
This notebook demonstrates supervised regression on physical measurement data.  
Included steps:

- Data visualization  
- Polynomial and linear regression  
- Model comparison  
- Interpretation of measurement behavior  

---

## 📂 3. Unsupervised Learning

### 🤖 Unsupervised Representation Learning for Depth Data  
**Notebook:** `Autoencoder_PCA.ipynb`  
**Dataset:** `Messreihe_demo1.csv`

**Summary:**  
This project explores unsupervised representation learning on depth profiles captured by a sensor system.  
Key methods:

- **Principal Component Analysis (PCA)** as a linear baseline  
- **Autoencoder** as a nonlinear deep-learning approach  
- **k-Means clustering** in both PCA and Autoencoder latent spaces  
- **Manifold analysis** and visualization  
- **Evaluation of reconstruction errors**  
- **Interpretation of continuous transformations** in depth measurements

**Limitations:**  
The depth profiles had inconsistent lengths. To obtain a uniform matrix representation, all profiles were trimmed to match the shortest sequence. While this ensured compatibility with PCA and Autoencoders, the trimming process may have altered the spatial continuity of the scans. Depth values often encode structured pixel or scan-line relationships, and cutting sequences can shift boundaries or truncate meaningful transitions. This likely influenced the learned manifold in PCA and the Autoencoder.

A more robust dataset with consistent spatial formatting—or preprocessing methods such as interpolation instead of raw trimming—would preserve local variations more accurately.

**Future improvements:**

- Use a dataset with fixed-length depth grids or structured pixel maps  
- Apply convolutional or variational autoencoders to model spatial structure  
- Explore point-cloud methods such as **PointNet**  
- Collect data with controlled physical parameters (e.g., angle, distance) for validation  

---

## 📁 Repository Structure

```
Kaggle Projects/
│── BBC News Classification.ipynb
│── BBC News Train.csv
│── BBC News Test.csv
│── BBC News Sample Solution.csv

Supervised Learning/
│── ML-demo1.ipynb
│── Messreihe_demo1.csv

Unsupervised Learning/
│── Autoencoder_PCA.ipynb
│── Messreihe_demo1.csv

README.md
```

---

## 🛠️ Technologies Used
- Python 3  
- pandas  
- NumPy  
- scikit-learn  
- matplotlib  
- seaborn  
- PyTorch  
- Jupyter Notebook  

---

## ▶️ How to Run
1. Clone or download this repository  
2. Install required Python packages  
3. Ensure datasets are in the correct subfolders  
4. Open the notebooks  
5. Execute all cells in order  

---

## 📄 License
This repository is intended for educational and academic purposes.
