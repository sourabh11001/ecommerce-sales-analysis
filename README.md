# 🛒 Sales Data Analysis & Customer Segmentation (RFM Analysis)

## 📌 Project Overview
This project analyzes **e-commerce sales transaction data** to uncover key business insights and segment customers using **RFM analysis** (Recency, Frequency, Monetary value).  

It simulates a real-world business problem where an e-commerce company wants to:
- Identify their most valuable customers  
- Understand sales trends  
- Improve marketing strategies and retention  

---

## 📂 Dataset
- **File:** `data.csv`  
- **Key Columns:**  
  - `InvoiceNo` – Invoice number (unique per transaction)  
  - `StockCode` – Product code  
  - `Description` – Product name  
  - `Quantity` – Number of items purchased  
  - `InvoiceDate` – Date of purchase  
  - `UnitPrice` – Price per item  
  - `CustomerID` – Unique customer identifier  
  - `Country` – Customer location  

---

## 🛠 Tools & Libraries Used
- **Python** – Data manipulation & analysis  
- **Pandas** – Data cleaning & transformation  
- **Matplotlib & Seaborn** – Data visualization  
- **Google Colab / Jupyter Notebook** – Development environment  
- **Plotly (optional)** – Interactive charts  

---

## 📊 Analysis Steps

### 1️⃣ Data Cleaning & Preprocessing
- Removed missing values (especially `CustomerID`)  
- Removed canceled orders (`InvoiceNo` starting with `"C"`)  
- Converted `InvoiceDate` to datetime format  
- Created new column `TotalPrice = Quantity × UnitPrice`  

### 2️⃣ Exploratory Data Analysis (EDA)
- Top-selling products  
- Monthly sales trends  
- Revenue by country  
- Which product sold the most in each month  
- **Visualizations:** bar charts, line graphs, pie charts  

### 3️⃣ RFM Analysis – Customer Segmentation
- **Recency (R):** Days since last purchase  
- **Frequency (F):** Number of transactions  
- **Monetary (M):** Total spending  
- Scored customers on a scale of **1–5** for each metric  
- Created **RFM Score** (e.g., `555` = best customers)  

### 4️⃣ Customer Segments

| Segment         | Description                                   |
|-----------------|-----------------------------------------------|
| **Champions**   | Recent, frequent, high-spending customers     |
| **Loyal**       | Purchase often, strong brand loyalty          |
| **Big Spenders**| Spend a lot, even if not very frequent        |
| **At Risk**     | Haven’t purchased in a long time              |
| **Recent**      | New customers making first purchases          |
| **Others**      | Low-value or inactive customers               |

---

## 📈 Key Insights (From Dataset)
- **Top 5 Products:** To be analyzed from dataset  
- **Peak Sales Month:** To be identified  
- **Country with Most Revenue:** To be identified  
- **Champions Segment:** X% of customers, contributing Y% of revenue  
- **At Risk Customers:** Identified for re-engagement campaigns  

---

## 📷 Sample Visualizations
(Add plots as PNG in `/images/` folder)  

Example:  
- `images/monthly_sales.png`  
- `images/rfm_segments_pie.png`  
- `images/top_products.png`  

---

## 🚀 How to Run

Clone this repository:
```bash
git clone https://github.com/yourusername/ecommerce-data-analysis.git
```

Open `analysis.ipynb` in **Google Colab** or **Jupyter Notebook**  

Install dependencies if needed:
```bash
pip install pandas matplotlib seaborn plotly
```

Run all cells to reproduce the analysis  

---

## 📌 Future Improvements
- Create interactive dashboard using **Plotly** or **Power BI**  
- Automate RFM scoring and generate monthly reports  
- Implement predictive modeling for customer churn  

---

## 📜 License
This project is open-source and available under the **MIT License**.  
