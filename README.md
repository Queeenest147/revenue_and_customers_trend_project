# Revenue & Customer Trends Analysis

## 1. Executive Summary
This project transformed over 200,000 fragmented sales transactions into a centralized Management Information System (MIS) that delivers both operational visibility and strategic insight. By integrating advanced techniques such as RFM Analysis, Price Elasticity, and Scenario Planning, the analysis moved beyond basic reporting to enable data-driven decision-making.

The solution eliminated manual reporting inefficiencies, uncovered high-value customers driving a disproportionate share of revenue, and introduced data-backed pricing strategies to reduce uncertainty. As a result, the project provided a clear pathway for profit optimization, targeted customer engagement, and risk-aware business planning, including tools to forecast the financial impact of pricing decisions before implementation.

## 2. Project Overview
2. Project Overview
   
This project is set within the E-commerce and Global Retail sector, focusing on Business Intelligence and Customer Analytics. It analyzes high-volume transactional data to understand purchasing behavior, product performance, and revenue patterns.

The business operates in a complex environment with 200,000+ international transactions, multiple product categories, and a diverse customer base. However, the lack of a centralized data system made it difficult to identify high-profit products, loyal customers, and true revenue drivers.

This project addresses these challenges by transforming raw data into a structured analytical system that supports proactive decision-making. Through techniques like RFM Analysis and Price Elasticity, it helps the business optimize pricing, focus on high-value customers, and allocate resources more effectively.

Ultimately, the solution improves operational efficiency, profitability, and scalability, enabling the business to shift from manual reporting to a data-driven strategy for growth.

## 3. Data Source
* Data Source: Kaggle (E-commerce transaction dataset)

* Dataset Size: 224,373 rows and 13 columns

* Data Type: Transactional data stored in an Excel workbook (each row represents a single sales transaction)

* Limitations:

- The dataset is static and not connected to a real-time database

- Analysis is limited to historical data (2018–2019) and may not reflect current trends

- Customer IDs may represent organizations rather than individual buyers
  
## 4. Problem Statement


**What is the issue?**
The core issue was Information Overload without Intelligence. Despite generating over 224,000 transaction rows, the business lacked a structured way to interpret this data. Operational logs were treated as a digital "filing cabinet" rather than a strategic asset, leading to fragmented reporting and a disconnect between sales activities and financial outcomes.


**Why is it important?**
In a high-volume retail environment, inefficiency is expensive. Without a centralized system:

* Time is wasted: High-level analysts were spending their time cleaning data instead of interpreting it.

* Profit is lost: The business risked over-stocking low-margin items while neglecting the "Super-fans" who drive the majority of the revenue.

* Risky Decision Making: Changing prices or inventory levels without a "What-If" model is essentially guesswork, which can lead to catastrophic revenue drops or missed opportunities for growth.


**What questions are we trying to answer?**
To solve these issues, this project was designed to answer three critical business questions:

* Revenue Concentration: Which specific products and geographic regions represent the "engine" of our growth, and which are underperforming?

* Price Sensitivity: If we adjust our pricing strategy, which products will maintain their sales volume (Inelastic) and which will see a sharp decline (Elastic)?

* Customer Valuation: Who are our most valuable customers based on the RFM (Recency, Frequency, Monetary) model, and how can we tailor our retention strategies for them?


**Key Questions Addressed:**
1. Which hardware and product categories drive the highest revenue?
2. How do price changes affect the demand for top-selling items?
3. Which customer segments contribute the most to the bottom line (Pareto Principle)?


## 5. Tools & Methodology

* **Tool Used:** Microsoft Excel.

* **Methodology & Technical Workflow**
  
The project followed a rigorous data pipeline to ensure that raw Kaggle data was transformed into reliable business intelligence.

**I. Data Collection**
* Source: Acquired secondary transactional data from Kaggle.

* Initial State: The raw dataset required significant structuring to align with business logic and financial reporting standards.

**II. Data Cleaning & Preparation**

* Standardization: Removed inconsistent formats and duplicates to ensure every transaction was unique.

* Data Type Integrity: Verified that all numerical values (Price, Quantity) were correctly typed to prevent calculation errors.

* Handling Missing Values: Addressed null values using aggregation techniques to maintain dataset volume without compromising accuracy.

* Feature Engineering: Decomposed the Date column into Day, Month, Year, and Weekday. This operation allowed for granular time-series analysis and seasonal trend identification.

**III. Data Transformation & Modelling**

* Advanced Calculations: * RFM Analysis: Categorized customers by Recency, Frequency, and Monetary value.

* Price Elasticity: Calculated the log-log relationship between price changes and demand.

* DAX Measures: Authored custom DAX formulas, including Average Revenue Per Customer and Total Revenue.

* Scenario Manager: Built a "What-If" analysis tool to forecast outcomes based on price and quantity fluctuations.

**IV. Data Validation**

* Integrity Checks: Cross-referenced KPI values against raw aggregates to ensure consistency across all dashboard slices.

* Logic Verification: Verified that the sum of departmental and country-level revenue is equal to the total organizational revenue.


## 6. Exploratory Data Analysis (EDA)

The exploratory analysis focused on understanding revenue distribution, customer behaviour, and key business risks within a large multi-year dataset (224k+ rows).

**Key Findings**

* Revenue Concentration (Pareto Effect):
A small percentage of customers contribute a disproportionate share of total revenue, highlighting the importance of high-value customer retention.

* Outlier Detection:
A major outlier (Customer ID 16446) was identified, contributing a significant portion of total revenue. This indicates a high dependency risk on key customers.

* Geographic Distribution:
Revenue is heavily concentrated in the United Kingdom, with additional strong performance observed in countries like the Netherlands, France, Norway, and Japan, suggesting potential growth opportunities.

Temporal Trends:
Sales performance improved in 2019 compared to 2018, with a clear seasonal peak in September, indicating a recurring demand cycle.

Price Sensitivity & Correlation:
While demand generally decreases as price increases, certain product categories show low price sensitivity (inelastic demand), presenting opportunities for price optimization and higher profit margins.

## 7. Key Insights

### Insight 1: The September Revenue Surge

**What happened?**

Revenue peaked significantly in September 2019, becoming the highest-performing month in the dataset.

**Why did it happen?** 

This was driven by a massive volume spike in the "Paper Craft" category, specifically the "Paper Craft Little Birdie" which moved over 80,000 units in that window alone.

**Why does it matter?** 

This reveals a strong seasonal demand cycle. By identifying this "Buying Season" in advance, the business can optimize supply chain logistics and marketing spend to ensure they don't face stock-outs during this high-velocity period.

### Insight 2: The "Super-Fan" Concentration Risk

**What happened?**

A single customer (ID 16446) contributed a staggering $1,002,718 in revenue—roughly 36% of the total business revenue.

**Why did it happen?** 

This customer represents a high-frequency, high-volume buyer (likely a B2B or wholesale distributor) who relies on specific product lines.

**Why does it matter?** 

While this revenue is great, it represents a High Concentration Risk. If this one customer leaves, the business loses over a third of its income. This insight shifts the strategy from "Mass Marketing" to "Key Account Management" and VIP retention.

### Insight 3: Price Elasticity & Margin Opportunities

**What happened?** 

Modelling showed that "World War 2 Gliders" are Elastic (Price Sensitive), while "Popcorn Holders" are Inelastic (Price Insensitive).

**Why did it happen?** 

Customers view "Popcorn Holders" as a necessity or a low-cost add-on where a small price increase isn't noticed, whereas the "Gliders" are treated as price-sensitive discretionary items.

**Why does it matter?** 

This is a Profit Roadmap. The business can safely raise prices on "Inelastic" goods to increase margins without losing customers. Conversely, they should use "Elastic" goods as "Loss Leaders" or keep prices stable to maintain volume.

## 8. Dashboard Preview

Visual Type 1: Dashboard Screenshots 

<img width="1133" height="434" alt="Screenshot 2026-03-19 164850" src="https://github.com/user-attachments/assets/83ab47cf-cde6-46d4-bb93-22da75591cc0" />

**Visual Type 2: After Data Cleaning**

<img width="1122" height="446" alt="image" src="https://github.com/user-attachments/assets/efb8956e-957d-4726-b164-43de0d3fa2b9" />

**Visual Type 3: Insight Visualization with Interpretation**

**Customers that generate the most Revenue**

<img width="228" height="134" alt="Screenshot 2026-03-19 165306" src="https://github.com/user-attachments/assets/f748f90b-05dc-4717-8ded-7cfd9ba5903a" />

**Countries that made the Highest Sales**

<img width="411" height="147" alt="Screenshot 2026-03-19 165317" src="https://github.com/user-attachments/assets/105c688d-7984-4626-92ae-bd17e347792e" />

**Products that Generate more Revenue **

<img width="445" height="169" alt="Screenshot 2026-03-19 165333" src="https://github.com/user-attachments/assets/c46fcd1e-4d66-4313-8858-f24a1fbe9ab3" />


**Revenue Distribution by Countries**

<img width="345" height="184" alt="image" src="https://github.com/user-attachments/assets/ed9f9079-2597-4f5a-bf16-5eb2c62c85f9" />

### Visual Type 4: Process Flow Diagram 

<img width="1024" height="1536" alt="image" src="https://github.com/user-attachments/assets/b7ecf5b4-d690-43fc-80fb-64bb9a1a8f41" />


## 9. Strategic Recommendations

### 1. Optimize High-Margin Product Pricing

* Action: Adjust prices upward (about 5–10%) for products identified as inelastic.

* Strategy: These products have low price sensitivity, so a controlled price increase can improve profit margins without significantly reducing sales volume.

* Business Impact: Higher revenue and improved profitability from existing demand.

### 2. Implement a VIP Loyalty Program

* Action: Focus retention efforts on the top 5% of customers using exclusive rewards and targeted incentives.

* Strategy: Prioritize retaining high-value customers since they contribute a large share of revenue and are more cost-effective to keep than acquiring new ones.

* Business Impact: Increased customer retention, stronger loyalty, and stable recurring revenue.

### 3. Inventory Rebalancing for Peak Periods

* Action: Increase inventory for top-selling products at least 30 days before peak demand periods (e.g., September and October).

* Strategy: Use demand patterns to anticipate high-sales periods and ensure adequate stock availability.

* Business Impact: Reduced stock-outs, improved sales fulfillment, and maximized revenue during peak demand.

## 10. Limitations & Assumptions

* The analysis is based on a static Excel dataset, meaning it requires manual updates and does not support real-time data syncing.

* It assumes each “Customer ID” represents an individual buyer, although it may actually reflect group or organizational purchasing behavior.

* The results are largely influenced by data from the United Kingdom, which may limit how well the insights apply to other regions without proper segmentation.

## 11. Implementation & Action Plan

### Phase 1: Strategic Deployment (Roadmap)

To move this project from a prototype to a production-ready system:

**What needs to be done?**

Transition the current Excel-based solution into a SQL-integrated Power BI environment to enable real-time reporting and scalability. Also, expand and deploy the VIP Loyalty Program using insights from the RFM analysis.

**Who is responsible?**

* Execution: Data Analytics Team

* Oversight: Finance and Sales Teams

**When should it happen?**

Immediate implementation in Quarter 3 (Q3) to prepare for the September peak period.

**How will success be measured?**

* Elimination of manual reporting processes (target: 100% reduction)

* Increase in profit margins by 5–10% through optimized pricing strategies

**What resources are required?**

* Power BI licenses

* SQL database access

* Historical CRM data for improved customer segmentation

### Phase 2: Risk Management (What could go wrong?)

**Data Drift:** Market conditions can change over time, which may affect the accuracy of current assumptions (e.g., products previously considered inelastic may become price-sensitive). Continuous monitoring is required.

**Over-reliance on Key Customers:** Heavy dependence on a small group of high-value customers (Super-fans) can be risky. A drop in these accounts could significantly impact revenue, so customer acquisition strategies must also be maintained.

## 12. Conclusion
This project addressed the challenge of having large amounts of transaction data without clear, actionable insights. By analyzing over 224,000 transactions, the data was transformed into meaningful insights that support better business decisions.

The analysis showed that a small group of high-value customers drives a large share of revenue, while certain products are less sensitive to price changes and can support margin improvements. These findings help the business focus on both customer retention and pricing strategy to improve performance.

Overall, this project delivers a practical Management Information System (MIS) that shifts the business from reactive reporting to more proactive, data-driven decision-making.

## 13. Relevant Links & Table of Contents

| Section Number | Navigation Link | Description |
| :--- | :--- | :--- |
| 1 | [Executive Summary](#1-executive-summary) | High-level project overview and impact. |
| 2 | [Project Overview](#2-project-overview) | Industry context and business domain. |
| 3 | [Data Source](#3-data-source) | Origin, size, and limitations of the dataset. |
| 4 | [Problem Statement](#4-problem-statement) | Challenges addressed and key business questions. |
| 5 | [Tools & Methodology](#5-tools--methodology) | Technical workflow and software used. |
| 6 | [Exploratory Data Analysis](#6-exploratory-data-analysis-eda) | Key findings, outliers, and trends. |
| 7 | [Key Insights](#7-key-insights) | Deep dive into revenue spikes and elasticity. |
| 8 | [Dashboard Preview](#8-dashboard-preview) | Visual gallery of the MIS prototype. |
| 9 | [Strategic Recommendations](#9-strategic-recommendations) | Actionable advice for profit optimization. |
| 10 | [Limitations & Assumptions](#10-limitations--assumptions) | Scope and technical constraints. |
| 11 | [Implementation & Action Plan](#11-implementation--action-plan) | Roadmap for deployment and risk management. |
| 12 | [Conclusion](#12-conclusion) | Final reflections and business value. |

---
[Back to Top](#revenue--customer-trends-analysis)
