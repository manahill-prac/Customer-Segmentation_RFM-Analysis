# 🛍 Customer Segmentation with RFM Analysis  

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/manahill-prac/ElevvoPathways_Customer-Segmentation_RFM-Analysis/blob/main/notebooks/RFM_Analysis.ipynb)

This project applies **RFM Analysis (Recency, Frequency, Monetary)** to segment customers from the **Online Retail Dataset (UCI ML Repository)**.  
The goal is to identify customer groups, generate actionable insights, and suggest marketing strategies.  


## 📊 Dataset  

- **Source**: [Online Retail Dataset – UCI ML Repository](https://archive.ics.uci.edu/ml/datasets/online+retail)  
- **File**: `Online Retail.xlsx`  
- **Fields**: `InvoiceNo, InvoiceDate, CustomerID, Quantity, UnitPrice, Country`  


## 🚀 How to Run  

1. **Clone the repository**  
   ```bash
   git clone https://github.com/manahill-prac/ElevvoPathways_Customer-Segmentation_RFM-Analysis.git
   cd ElevvoPathways_Customer-Segmentation_RFM-Analysis
````

2. **Open in Google Colab** using the badge above or manually.

3. **Mount Google Drive** inside Colab:

   ```python
   from google.colab import drive
   drive.mount('/content/drive')
   ```

4. **Load dataset**:

   ```python
   file_path = "/content/drive/MyDrive/ColabDatasets/Online Retail.xlsx"
   df = pd.read_excel(file_path)
   ```

5. Run all cells in `RFM_Analysis.ipynb`.

---

## 🧮 RFM Analysis Steps

1. **Data Cleaning**

   * Removed nulls, duplicates, negative quantities
   * Converted datatypes

2. **RFM Metrics Calculation**

   * **Recency (R):** Days since last purchase
   * **Frequency (F):** Number of purchases
   * **Monetary (M):** Total spend

3. **Scoring & Segmentation**

   * Scaled RFM scores (1–5)
   * Created segments (*Champions, Loyal, At Risk, Lost, etc.*)

4. **Visualization**

   * Heatmaps of RFM segments
   * Bar charts of customer distribution

5. **Insights & Recommendations**

   * *Champions*: Reward loyalty with VIP perks
   * *Loyal Customers*: Provide personalized offers
   * *At Risk*: Use win-back campaigns
   * *Lost Customers*: Re-engage with minimal cost

---

## 📦 Dependencies

Install dependencies via:

```bash
pip install -r requirements.txt
```

Main libraries:

* pandas
* numpy
* matplotlib
* seaborn
* openpyxl

---
