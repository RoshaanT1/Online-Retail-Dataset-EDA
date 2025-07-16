# Online Retail Dataset - Exploratory Data Analysis (EDA)

## 📊 Project Overview

This project performs comprehensive exploratory data analysis on the Online Retail II dataset to uncover insights about customer behavior, sales patterns, and business performance. The analysis includes data cleaning, outlier removal, trend analysis, and customer segmentation using RFM (Recency, Frequency, Monetary) methodology.

## 📁 Project Structure

```
dataAnaylsis2/
├── README.md                    # Project documentation
├── dataAnalysis.ipynb          # Main Jupyter notebook with EDA
├── online_retail_II.xlsx       # Original dataset
└── visualization.pbix          # Power BI visualization file
```

## 📈 Dataset Description

The Online Retail II dataset contains transactional data from a UK-based online retail company. This dataset is sourced from Kaggle: [Online Retail Dataset](https://www.kaggle.com/datasets/lakshmi25npathi/online-retail-dataset).

The dataset includes the following columns:

- **Invoice**: Invoice number (6-digit integral number)
- **StockCode**: Product code (5-digit integral number)
- **Description**: Product name
- **Quantity**: Quantities of each product per transaction
- **InvoiceDate**: Invoice date and time
- **Price**: Unit price of products
- **Customer ID**: Customer number (5-digit integral number)
- **Country**: Country name where customer resides

## 🔍 Analysis Performed

### 1. Data Cleaning & Preprocessing
- ✅ Removed duplicate records
- ✅ Filtered out cancelled invoices (starting with 'C')
- ✅ Handled missing values in Customer ID column
- ✅ Outlier detection and removal using IQR method for Quantity and Price columns

### 2. Exploratory Data Analysis
- **Product Analysis**
  - Number of unique products
  - Top 10 selling products by quantity
  - Top 10 revenue-generating products
  
- **Customer Analysis**
  - Total number of unique customers
  - Top 5 customers by purchase quantity
  - Customer purchase distribution and loyalty analysis
  
- **Geographic Analysis**
  - Top countries by customer count
  - Sales distribution by country
  - Revenue percentage by country

### 3. Time Series Analysis
- Monthly sales trends
- Daily sales patterns
- Weekly sales trends

### 4. Customer Segmentation
- **RFM Analysis** (Recency, Frequency, Monetary)
  - Recency: Most recent purchase date per customer
  - Frequency: Number of purchases per customer
  - Monetary: Total revenue generated per customer

## 📊 Key Findings

- **Dataset Size**: After cleaning, the dataset contains thousands of transactions
- **Geographic Distribution**: UK dominates the customer base and revenue
- **Seasonal Patterns**: Clear monthly and weekly trends in sales
- **Product Performance**: Identification of top-performing products by volume and revenue
- **Customer Insights**: Customer segmentation reveals purchasing patterns and loyalty

## 🛠️ Technologies Used

- **Python 3.13.1**
- **Libraries**:
  - `pandas` - Data manipulation and analysis
  - `matplotlib` - Data visualization
  - `openpyxl` - Excel file handling
- **Power BI** - Advanced data visualization
- **Jupyter Notebook** - Interactive data analysis environment

## 🚀 Getting Started

### Prerequisites
```bash
pip install pandas matplotlib openpyxl
```

### Running the Analysis
1. Clone or download this repository
2. Open `dataAnalysis.ipynb` in Jupyter Notebook or VS Code
3. Run all cells sequentially to reproduce the analysis
4. The cleaned dataset will be saved as `online_retail_II_cleaned.csv`

### Power BI Dashboard
Open `visualization.pbix` in Power BI Desktop to explore interactive visualizations and dashboards.

## 📋 Analysis Steps

1. **Data Loading**: Import Excel dataset using pandas
2. **Data Exploration**: Check data types, missing values, and basic statistics
3. **Data Cleaning**: Remove duplicates, filter cancelled orders, handle outliers
4. **Statistical Analysis**: Generate descriptive statistics and insights
5. **Visualization**: Create various plots for trend analysis
6. **Customer Segmentation**: Perform RFM analysis
7. **Export Results**: Save cleaned data for further use

## 🎯 Business Insights

The analysis provides valuable insights for:
- **Inventory Management**: Understanding top-selling products
- **Customer Retention**: Identifying loyal customers through RFM analysis
- **Market Strategy**: Geographic revenue distribution
- **Sales Forecasting**: Historical trends and patterns
- **Product Strategy**: Revenue vs. volume analysis

## 📝 Future Enhancements

- [ ] Advanced customer segmentation using clustering algorithms
- [ ] Predictive modeling for customer lifetime value
      
## 👥 Contributing

Feel free to fork this project and submit pull requests for improvements or additional analysis.

## 📄 License

This project is for educational and analytical purposes. Please ensure proper attribution when using the dataset or code.

