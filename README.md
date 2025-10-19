# 🧠 Business Intelligence Solution for Purchasing Department (AdventureWorks)

## 📘 Overview
This project is part of the **Business Intelligence and Decision Support System** course at the **University of Economics and Law (VNUHCM)**.  
It focuses on **building a complete Business Intelligence (BI) solution** for the **Purchasing Department** of the **AdventureWorks Company**, using Microsoft BI technologies to support procurement decision-making and performance evaluation.


---

## 🎯 Project Objectives
- Develop a **Business Intelligence solution** to enhance purchasing decision-making.  
- Analyze procurement performance and vendor reliability.  
- Optimize purchasing costs, delivery time, and stock efficiency.  
- Build an end-to-end BI architecture including **ETL, data warehouse, OLAP, and dashboards**.  

---

## 🏗️ Project Architecture
**Tools & Technologies Used:**
- **SQL Server Management Studio (SSMS)** – Database management and querying  
- **SQL Server Integration Services (SSIS)** – ETL (Extract, Transform, Load) processes  
- **SQL Server Analysis Services (SSAS)** – Cube building and OLAP analysis  
- **Power BI** – Data visualization and interactive dashboards  

**Architecture Layers:**
1. **Data Source Layer:** AdventureWorks database (OLTP)  
2. **ETL Layer:** Extract, transform, and load purchasing data into Data Mart using SSIS  
3. **Data Warehouse Layer:** Star schema with Fact and Dimension tables  
4. **OLAP Layer:** SSAS cube for multidimensional analysis  
5. **Visualization Layer:** Power BI dashboards for KPIs and decision support  

---

## 🧩 Data Model
The data warehouse follows a **Star Schema** design:

**Fact Table:**
- `FactPurchaseOrder`

**Dimension Tables:**
- `DimVendor`  
- `DimProduct`  
- `DimEmployee`  
- `DimShipMethod`  
- `DimProductVendor`  
- `DimInventory`  
- `DimTime`
<img width="576" height="537" alt="image" src="https://github.com/user-attachments/assets/ed13f202-a547-4941-8825-efb77ccc57f3" />

---

## 📊 Key Performance Indicators (KPIs)
| KPI | Description |
|-----|--------------|
| **Total Purchase Orders** | Number of purchase orders issued in a period |
| **Total Stock Quantity** | Total quantity of goods purchased |
| **Average Lead Time** | Average days from order to delivery |
| **Fulfillment Rate** | Percentage of orders delivered on time |
| **Top Vendors by Value** | Ranking of suppliers based on order amount |
| **Purchase Cost Trend** | Monthly or yearly trend of procurement costs |

---
## DashBoard
There are 5 dashboard for purchasing department
<img width="960" height="538" alt="image" src="https://github.com/user-attachments/assets/2d3b60d9-f84d-4dca-bbd8-ddc9a9827db0" />

<img width="959" height="538" alt="image" src="https://github.com/user-attachments/assets/ba14f828-29e0-49b6-b04c-ca417488adc8" />

<img width="956" height="537" alt="image" src="https://github.com/user-attachments/assets/b6672767-fc33-4b2a-b256-4ed9a83bdc88" />

<img width="957" height="540" alt="image" src="https://github.com/user-attachments/assets/4d7ad0d9-5a0b-4835-8fef-16b2a49a9cbb" />

![Uploading image.png…]()


## 💡 Features
- Extract purchasing data from AdventureWorks database.  
- Transform and clean data using SSIS workflows.  
- Build OLAP cube with SSAS for multidimensional analysis.  
- Create interactive Power BI dashboards for:
  - Vendor performance comparison  
  - Delivery timeliness  
  - Procurement spending trends  
  - Purchase cycle analysis  

---

## ☁️ Deployment
- The project can be deployed on **SQL Server** with **SSISDB** integration.  
- **SQL Server Agent Jobs** are used to automate ETL executions.  
- Power BI dashboards are published via **Power BI Service** for sharing and cloud access.  

---

## 📂 Project Structure
```bash
📁 AdventureWorks-BI-Purchasing
┣ 📂 DataWarehouse
┃ ┣ star_schema_design.sql
┣ 📂 SSIS
┃ ┣ ETL_Packages
┃ ┣ Master_Pipeline.dtsx
┣ 📂 SSAS
┃ ┣ PurchasingCube.cube
┣ 📂 PowerBI
┃ ┣ PurchasingDashboard.pbix
┣ 📄 README.md
┣ 📄 report.pdf
