# 🛍️ E-commerce Sales Dashboard

### From messy retail transactions to actionable insights — an end-to-end data project with Python + Power BI
---

This project demonstrates how to **clean, prepare, and analyze e-commerce transaction data** using **Python (Pandas)** and build an **interactive dashboard in Power BI** to track revenues, cancellations, and product/category insights.

**This project was created entirely by me (data cleaning, feature engineering, dashboard design) as a portfolio piece.**

---

## Project Overview
The dataset contains real-world e-commerce transactions from [Kaggle](https://www.kaggle.com/datasets/carrie1/ecommerce-data) including:
- Invoice information
- Product descriptions
- Quantities and unit prices
- Customer IDs and country

The project involves:
1. Cleaning and preparing the raw dataset (handling missing values, returns, zero-priced items and noisy data).
2. Engineering new features such as product categories, return flags, and cancellations.
3. Creating an interactive **Power BI dashboard** for business insights.

---

## Data Source
This data was extracted from [Kaggle](https://www.kaggle.com/datasets/carrie1/ecommerce-data), it contains real-world data from a UK retail based company from 2010 to 2011. 
The data concerns only non-store online retail and the company typically sells unique all-occasion gifts. 

The image below shows the structure of the data and it contains 541909 data entry. 

<img width="1223" height="431" alt="image" src="https://github.com/user-attachments/assets/1700740d-4efe-4ece-aa6a-41afe9f9435b" />

## 🚀 Key Features
- 🧽 **Data Cleaning & Preparation**
  - Handle missing `CustomerID` and `Description`
  - Replace `NaN` descriptions with `"NO DESC"`
  - Convert IDs to integers with nullable support
  - Drop or flag zero-priced transactions
  - Flag returns (negative quantities) 
  - Handle incorrect descriptions
  - Drop the rows not concerning transactions
  - Categorize the data descriptions

- 📊 **Dashboard and Insights**
  The dashboard created here is only based on the figures and rates I wanted to show, however in real world the dashboard needs to cater more to the stakeholders' needs.
  - **KPIs:** Total Revenue, Number of Orders, Cancellation Rate
  - **Trends:** Daily revenues and orders over time
  - **Geography:** Orders by country
  - **Products:** Orders per product category

---

## 📊 Dashboard, Insights and recommendations
- **Dashboard Review**: It is important to mention that in this case that I could not use all the data from the file, since I didn't have enough space in my laptop. I was only able to use data from 4/11/2011 to 9/12/2011.

The global dashboard: 
<img width="973" height="555" alt="image" src="https://github.com/user-attachments/assets/e62f3b31-c420-4838-9e99-db7b5a1c617b" />

In the United Kingdom only:
<img width="987" height="553" alt="image" src="https://github.com/user-attachments/assets/3742e964-df6d-4f85-b004-fc97c819921a" />


- **Insights from the dashboard**:
    - **Most of the revenues and orders of this company is based only on UK**, this means that **the company is not very present internationally**.
    - Most of the products sold in this company fall within the "Miscellanous" category meaning **the company's products are versatile**. The categories were only created by me, so they still might need to be altered based on the company.
    - The cancellation rate is at 13.4% for the period between November and December. Since this rate is not high, there are probably **no problems with customer conversion rate**.
    - **The turnover is not very stable and does fluctuate.**
 
      
- **Recommendations**:
    - The company might need to **work more on its presence internationally especially european countries** (such as: Germany, France and Ireland), where they already have some presence but not enough.
    - The number of orders per day are below 200. This means that **the company needs to attract more customers using marketing campaigns or by proposing attractive products after carefully studying the market**.
      
- **Next Steps**:<br>
  After going through this data. I think the next steps should include:<br>
  - **Customer Segmentation**: Since the company does not get a lot of orders each day, a next step would be to **segment the customers and see if the company needs to attract new customers or propose discounts**.
  - **Study the competition**: This would help the company see the **prices proposed by competitors** for the same products as well as the **different products proposed**. 
---

## 🛠️ Tools & Technologies
- **Python**: pandas, numpy, matplotlib (data cleaning & prep), os and kagglehub (for data importing)
- **Power BI**: dashboard building
- **Git/GitHub**: version control and portfolio showcase
---

## 📂 Repository Structure
.<br>
├── notebooks/<br>
│   └── **Data Cleaning and Preparation for a Dashboard.ipynb**: This notebook showcases all the steps I took explore and handle data inconsistencies as well as introducing/removing columns depending on the dashboard use. Since this notebook contains all the small steps and details, **it is not for production**.<br>
├── dashboard/<br>
│   └── **Sales Insight Dashboard.pbix**: This is the dashboard I created using PowerBI, to showcase some insights for product teams for example.<br>
└── README.md

