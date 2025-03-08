# **CryptoClustering: K-Means & PCA for Cryptocurrency Analysis**

## **Project Overview**
This project applies **K-Means clustering** and **Principal Component Analysis (PCA)** to classify cryptocurrencies based on their price fluctuations over different timeframes. The goal is to identify meaningful patterns in the crypto market by leveraging **unsupervised machine learning** techniques.

## **Key Features**
- **Data Preprocessing:** Standardized cryptocurrency market data using `StandardScaler()`.
- **K-Means Clustering:**
  - Used the **Elbow Method** to determine the optimal number of clusters (`k`).
  - Applied **K-Means** to group cryptocurrencies based on their price changes.
- **Principal Component Analysis (PCA):**
  - Reduced the dataset to **three principal components**.
  - Re-evaluated the optimal `k` using the PCA-transformed data.
  - Clustered cryptocurrencies using **K-Means with PCA** and visualized the results.
- **Feature Analysis:** Identified which features had the **strongest positive and negative influence** on each principal component.

---

##  **Project Structure**
```
CryptoClustering/
│── crypto_market_data.csv        # Dataset used for analysis
│── Crypto_Clustering.ipynb       # Jupyter Notebook with full analysis
│── README.md                     # Project documentation (this file)
└── requirements.txt               # Dependencies for running the project
```

---

## **Technologies & Libraries**
This project was built using the following Python libraries:
- `pandas` - Data manipulation and analysis
- `matplotlib` - Data visualization
- `scikit-learn` - Machine learning models (`KMeans`, `PCA`, `StandardScaler`)

---

## **Results & Insights**
### **Optimal Number of Clusters (Elbow Method)**
- Before PCA: **k = 6**
- After PCA: **k = 4** 
- PCA significantly improved clustering by reducing noise and redundancy.

### **Feature Influence on Principal Components**
- **PC1:** Most influenced by `price_change_percentage_200d` (0.5945) and `price_change_percentage_24h' (-0.4167).
- **PC2:** Most influenced by `price_change_percentage_30d` (0.5622) and `price_change_percentage_1y` (-0.1508).
- **PC3:** Most influenced by `price_change_percentage_7d` (0.7877) and `price_change_percentage_60d` (-0.3614).

_→ These findings help us understand which factors drive cryptocurrency price changes over time._

---

## 🏆 **Key Takeaways**
- **K-Means clustering** effectively groups cryptocurrencies based on price behavior.
- **PCA reduces dimensionality** while preserving significant variance, improving clustering efficiency.
- **Feature influence analysis** reveals the strongest market drivers affecting cryptocurrency price changes.

## 📜 **License**
This project is open-source and available under the **MIT License**.

---

### 🌟 **Contact**
Jill Balderson (JBalderson-AI)



