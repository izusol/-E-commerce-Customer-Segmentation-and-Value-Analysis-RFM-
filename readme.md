# **E-commerce Customer Segmentation and Value Analysis (RFM)**

## **Project Overview**

This project focuses on applying the **RFM (Recency, Frequency, Monetary)** model to a large, real-world e-commerce transactional dataset ( rows). The primary objective was to move beyond simple revenue analysis, segment the customer base into actionable groups, and identify critical retention opportunities.

## **Technical Execution**

The analysis was performed end-to-end using **Python and the Pandas library**, demonstrating a robust data science workflow from cleaning to interpretation.

### **Key Steps:**

1. **Data Cleaning:**  
   * Handled over  missing CustomerID records (crucial for segmentation).  
   * Corrected type issues (string dates to datetime, float IDs to int).  
   * Filtered out all cancellation records ('C' in InvoiceNo) and invalid transactions ().  
2. **RFM Calculation:**  
   * Calculated raw R, F, and M metrics for each unique customer.  
   * Used the pd.qcut function with duplicates='drop' to robustly assign scores (1-5) based on quintiles, creating the final RFM\_Score.  
3. **Segmentation & Visualization:**  
   * Applied custom business logic to assign customers to 7 strategic segments (e.g., BestCustomers, New Customers, Lost Customers).  
   * Generated visualizations (Bar and Pie charts) to summarize customer count and revenue contribution by segment.

## **Core Findings**

The segmentation revealed a serious retention problem masked by high acquisition:
  
* **Acquisition Focus:** The **"New Customers"** segment is the largest (), indicating strong acquisition but weak immediate follow-up.

## **Business Recommendation**

The business is advised to immediately shift focus and budget toward a **90-day New Customer Onboarding and Retention Campaign** to convert the large pool of "New Customers" into "Loyal Customers," thereby stabilizing long-term revenue.

**Technologies Used:** Python, Pandas, Matplotlib/Seaborn
