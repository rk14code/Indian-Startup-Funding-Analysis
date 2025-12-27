# 🚀 Indian-Startup-Funding-Analysis (2015–2020)
## 📌 Project Overview

This project presents a comprehensive **exploratory data analysis (EDA)** of the **Indian startup funding ecosystem** from 2015 to 2020. The objective is to understand how startup funding has evolved over time and to identify key patterns across **industries**, **locations**, **funding types**, **investors**, and **startup maturity**.

A major focus of this project is **real-world data cleaning and standardization**, addressing inconsistencies, missing values, encoding issues, and noisy categorical attributes. After building a clean and reliable dataset, in-depth EDA and visualization techniques are applied to extract meaningful insights that reflect investor behavior and startup growth trends in India.
___
## 🎯 Objectives

- Clean and standardize real-world startup funding data

- Understand the typical funding amount received by startups in India
  
- Analyze how startup funding trends change over time (year-wise analysis)

- Identify the most preferred industries and sub-industries

- Examine the role of geographic location in startup growth

- Identify key investors and dominant funding types

- Highlight startups and sectors attracting repeated and large-scale funding

- Derive business-relevant insights from EDA
___
## 📊 Dataset Description

Each row represents a startup funding event in India.

- **Rows:** 3,044

- **Columns:** 10

Key Columns:

- **Date** – The date when the funding was provided, in the format dd/mm/yyyy

- **Startup Name** – The name of the startup that received funding

- **Industry Vertical** – The industry or sector in which the startup operates, such as technology, healthcare, e-commerce, etc.

- **SubVertical** – A more specific category within the industry, providing additional details about the startup's focus

- **City** – The city or location where the startup is based

- **Investors Name** – The names of the investors or venture capital firms that provided the funding

- **Investment Type** –  The type of investment, such as Seed Funding, Series A, Series B, etc.

- **Amount in USD** → The amount of funding received by the startup, typically expressed in US dollars (later converted to Amount in Crore Rs.)

- **Remarks** –  Any additional remarks or notes about the funding round or the startup (later dropped)
___
## 🧹 Data Cleaning & Preprocessing

This project involves extensive real-world data preprocessing, including:

- **Data Type Corrections**

  - Converted date column to proper datetime formate

  - Cleaned funding amounts and converted them into INR (Crores)

- **Handling Missing Values**

  - Dropped high-missing and low-utility columns (e.g., Remarks)

  - Applied hierarchical imputation for missing funding amounts:

    - Industry-level median funding

    - Overall dataset median for remaining cases

- **Categorical Standardization**

  - Standardized Startup Names (e.g., Ola, OYO, Byju’s variants)

  - Cleaned encoding issues (\xc2\xa0, \xe2\x80\x99, etc.)

  - Normalized Industry Vertical, SubVertical, City, Investor Names

  - Unified inconsistent spellings and naming conventions using correction dictionaries

- **Entity-Level Consistency**

  - Grouped by Startup Name and assigned the most frequent:

    - Industry

    - Sub-industry

    - City

      This reduced noise and improved analytical consistency.

- **Final Clean Dataset**

  - Rows: 2,914

  - Columns: 9

  - No missing values in critical analytical fields
___
## 🛠️ Skills & Tools Used

- **Programming & Libraries**

  - Python: Pandas, NumPy

  - Visualization: Matplotlib, Seaborn

- **Techniques**

  - Data cleaning & validation

  - Encoding & text normalization

  - Hierarchical median imputation

  - Group-based aggregation

  - Statistical summaries

  - Business-driven EDA
___
## 🔎 Exploratory Data Analysis (EDA) – Key Insights

- **Funding Amount Distribution**

  - Funding amounts are highly right-skewed

  - Majority of startups receive small to moderate funding
 
  - A few mega-funding deals stretch the distribution up to ~₹35,000+ crore

  - Median funding (~₹14.37 crore) better represents a typical startup than the mean

- **Year-wise Funding Trends**

  - Peak funding observed in 2017 and 2019

  - Indicates strong investor momentum before economic slowdowns

  - Year-wise aggregation highlights cyclical investment behavior  

- **Top Startups by Funding**

  - Startups like Flipkart, Rapido, Paytm, Ola, Oyorooms, Udaan, Snapdeal dominate total funding

  - Startups like Ola, Paytm, Oyorooms, Swiggy, Byju’s, Urbanclap, Lendingkart and Lenskart appear repeatedly, reflecting multi-round funding cycles

- **Industry-Level Insights**

  - Consumer Internet, E-commerce, Technology, Finance and Logistics attract the most capital
 
  - Followed by Healthcare, Hospitality and Fin-Tech

  - Shows strong investor preference for scalable, digital-first platforms

- **Sub-Industry Analysis**

  - Bike Taxi, Online Marketplaces, Mobile Wallets & E-commerce lead funding

  - Platform-based business models attract the highest capital inflow

- **City-wise Analysis**

  - Bangalore is the undisputed startup hub (highest total, max funding, and startup count)

  - Mumbai, Gurugram, and New Delhi form the next tier

  - Presence of US cities highlights global investor participation
___
## 📈 Visualizations Used

- Funding distribution plots (Histogram + KDE)

- Year-wise funding trend line charts

- Bar charts for top startups, industries, sub-industries and cities

- Aggregation-based plots for funding comparison
___
## 📈 Business Value

- Helps investors identify high-growth sectors and cities

- Assists founders in understanding funding benchmarks

- Enables policymakers to evaluate ecosystem concentration

- Demonstrates how clean data improves strategic decision-making

- Bridges raw funding data with strategic business insights
___
## 📌 Conclusion

- This project demonstrates the importance of data cleaning before analysis when working with real-world datasets.
By combining rigorous preprocessing with structured EDA, the analysis uncovers meaningful patterns in startup funding across time, geography, and industries.

- The project highlights how thoughtful exploratory analysis can transform noisy startup data into insights that support investment decisions, market understanding, and strategic planning, making it highly relevant for Data Analyst and Data Scientist roles.
