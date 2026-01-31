# Customer Segmentation for Online Retail

## Project Overview

This project explores **customer segmentation** for a UK-based online retail company that sells unique all-occasion gifts. The goal is to group customers based on transactional behavior to better understand customer heterogeneity and enable **data-driven business decisions**.

Customer segmentation helps identify high-value, low-value, and wholesale-oriented customers, enabling personalized marketing, improved retention, and optimized promotions. This project applies **unsupervised machine learning (clustering)** techniques to uncover latent patterns in customer purchasing behavior.

---

## Business Objectives

* Identify **distinct customer segments** with similar transactional patterns
* Differentiate **retail and wholesale purchasing behaviors** using data-driven insights
* Enable **targeted marketing and communication strategies** tailored to each segment
* Improve **customer retention and long-term value** through personalized engagement
* Support **strategic decision-making** related to pricing, promotions, and customer management

**Business KPIs:**

* Clear and interpretable differentiation of customer segments
* Actionable segments for marketing, retention, and strategy
* Identification of high-value, low-value, and wholesale-oriented customer groups
* Support for downstream initiatives such as targeted promotions and personalized engagement

---

## Analytics Objectives

* Transform raw transactional data into **customer-level features** (RFM, quantity, variability)
* Handle **data cleaning and preprocessing**, including noise, returns, and anomalies
* Apply **clustering algorithms** to segment customers based on behavioral similarity
* Evaluate clustering results using internal validation metrics
* Profile and interpret clusters to ensure **business relevance and actionability**

**Technical KPIs:**

* **Silhouette Score** – measures cluster separation and cohesion for precise targeting
* **Within-Cluster Sum of Squares (WCSS)** – evaluates cluster compactness for reliable segment-specific actions
* **Davies-Bouldin Index** – assesses inter-cluster similarity to reduce misclassification
* **Stability and Interpretability** – ensures clusters are reproducible and actionable for decision-making

---

## Data

* Dataset: Publicly available **Online Retail Dataset** (UK-based, non-store retail, Dec 2010 – Dec 2011)
* Source: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/online+retail)
* Features include:

  * `InvoiceNo` – Invoice number
  * `StockCode` – Product code
  * `Description` – Product description
  * `Quantity` – Number of items per transaction
  * `InvoiceDate` – Date of transaction
  * `UnitPrice` – Price per item
  * `CustomerID` – Unique customer identifier
  * `Country` – Country of customer

---

## Methodology

1. **Data Preprocessing:**

   * Handle missing values, outliers, and returns
   * Aggregate transactional data to customer-level features (RFM analysis)

2. **Feature Engineering:**

   * Recency, Frequency, Monetary value, Quantity, and variability metrics

3. **Clustering Algorithms Explored:**

   * **K-Means** – simple and efficient clustering
   * **DBSCAN** – density-based clustering for irregular clusters and outliers
   * **Hierarchical Clustering** – visualize relationships between clusters
   * **Gaussian Mixture Models (GMM)** – probabilistic clustering with soft assignments

4. **Evaluation:**

   * Internal metrics: Silhouette Score, WCSS, Davies-Bouldin Index
   * Stability and interpretability checks
   * Translate clusters into **actionable business insights**

---

## Results

* Customer segments were identified with **clear distinctions in behavior**
* High-value, low-value, and wholesale-oriented segments were profiled
* Segments are actionable for **marketing, retention, and personalized engagement**
* Internal metrics confirm clusters are **well-separated, compact, and stable**

*Detailed analysis, visualizations, and cluster profiles are available in the Jupyter notebooks.*

---

## Scope and Future Work

**Scope:**

* Focused on **customer segmentation** using transactional data
* Market basket analysis, product-level recommendations, or association rules are **out of scope**

**Future Work:**

* Integrate **market basket analysis** for product bundling strategies
* Implement **recommendation systems** (collaborative or content-based filtering)
* Combine segmentation with **predictive modeling** for churn, high-value customers, or personalized promotions

---

## Project Structure

```
customer-segmentation/
├── src/                        
│   ├── data/                   # Raw and processed datasets
│   ├── models/                 # Saved clustering models
│   ├── notebooks/              # Jupyter notebooks for analysis
│   ├── requirements.txt        # Python dependencies
│   ├── LICENSE                 # Project license
│   └── README.md               # Project documentation
```

---

## Technologies Used

* Python 3.x
* Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn
* Jupyter Notebook

---

## How to Run

1. Clone the repository:

```bash
git clone https://github.com/yourusername/customer-segmentation.git
```

2. Navigate to `src/` and install dependencies:

```bash
pip install -r requirements.txt
```

3. Run notebooks in `notebooks/` to reproduce the analysis and results.

---

## License

This project is licensed under the MIT License.
