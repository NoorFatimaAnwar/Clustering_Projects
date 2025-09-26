# 📊 Customer Segmentation Using Kmeans

This project applies **Customer Segmentation** on an **online retail dataset** using RFM (Recency, Frequency, Monetary) analysis combined with clustering algorithms like **KMeans, Hierarchical Clustering, and DBSCAN**.  
The goal is to group customers into meaningful clusters for targeted marketing and business decision-making.  

---

## 📂 Project Structure
📁 Customer-Segmentation
│── 📓 customer_segmentation.ipynb # Jupyter Notebook (Colab code)
│── 📄 data.csv # Raw dataset (Online Retail)
│── 📘 README.md # Project documentation

---
## ⚙️ Steps Performed
1. **Data Loading & Cleaning**  
   - Handled missing values (`CustomerID`, `Description`)  
   - Converted `InvoiceDate` to datetime format  

2. **Feature Engineering (RFM Analysis)**  
   - **Recency**: Days since last purchase  
   - **Frequency**: Number of unique invoices per customer  
   - **Monetary**: Total amount spent  

3. **Outlier Handling**  
   - Removed extreme values using **IQR & percentile capping**  
   - Applied **log transformation** to reduce skewness  

4. **Scaling & Dimensionality Reduction**  
   - Used **StandardScaler** for normalization  
   - Applied **PCA** for 2D visualization  

5. **Clustering Models**  
   - **KMeans** (evaluated with Elbow method & cluster metrics)  
   - **Hierarchical Clustering (Agglomerative)**  
   - **DBSCAN** (density-based clustering)  

6. **Evaluation Metrics**  
   - Silhouette Score  
   - Calinski-Harabasz Index  
   - Davies-Bouldin Index  

7. **Visualization**  
   - PCA 2D plots of clusters  
   - 3D scatter plot with centroids  

---

## 📊 Example Results

- **Elbow Method** to find optimal clusters  
- **KMeans PCA Plot** with centroids  
- **3D Cluster Visualization** of Recency, Frequency, Monetary  

---

## 🛠️ Requirements
Install dependencies before running the notebook:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## ▶️ How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/Customer-Segmentation.git
   cd Customer-Segmentation
   ```

2. Open `customer_segmentation_Using_Kmeans.ipynb` in **Google Colab** or **Jupyter Notebook**  

3. Download the dataset (see **Dataset Link** section below) and place it in the project folder  

4. If running on **Colab**, upload `data.csv` manually  

5. Run all cells to perform preprocessing, clustering, and visualization  

---

## 📂 Dataset Link
Since the dataset is too large to upload in the repository, you can download it directly from here:  

👉 [Download Dataset](YOUR_DATASET_LINK_HERE)  

*(https://www.kaggle.com/datasets/carrie1/ecommerce-data)*  

---

## 🚀 Future Improvements
- Automate hyperparameter tuning for **DBSCAN** & **KMeans**  
- Try **Gaussian Mixture Models (GMM)** for soft clustering  
- Deploy clustering results into a dashboard (**Streamlit / Power BI**)  

---

## ✨ Author
👩‍💻 Developed by **Noor Fatima**  
📌 For learning and demonstration purposes (**Data Science / Customer Segmentation project**)  


**Developed by Noor Fatima**  
🎓 Final-year Computer Science Student | Data Science Projects  
