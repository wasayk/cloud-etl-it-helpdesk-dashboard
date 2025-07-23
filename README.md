# 🧰 IT Ticketing System Analytics (Cloud ETL + Power BI Project)

This project demonstrates a full cloud-native ETL + BI pipeline simulating an enterprise-grade ticketing system analysis.

It ingests raw support ticket data from Azure Blob Storage, transforms and loads it via Azure Data Factory into Azure SQL Database, and visualizes it using a Power BI dashboard. The solution is fully automated with scheduled refreshes.

---

## 🚀 Project Architecture
Raw Data (.CSV in Blob Storage)
↓
Azure Data Factory (ETL)
↓
Azure SQL Database (Structured Table)
↓
Power BI (Interactive Dashboard)

![image](https://github.com/user-attachments/assets/81785b1b-d1fd-4330-b16c-7c15b91e01ea)

## 🌐 Cloud ETL Components (Azure)

### 🟩 Azure Blob Storage
- Raw `.csv` file uploaded to `raw-data` container
- Simulates vendor/system raw data drop

### 🟧 Azure Data Factory
- Created a Copy Data pipeline
- Mapped source-to-sink fields with transformation
- Scheduled nightly data refresh

### 🟦 Azure SQL Database
- Cloud-hosted structured database
- Destination for cleaned IT ticket data
- Used as Power BI data source

- ## 🧾 SQL Queries & Insights

Before dashboarding, raw insights were explored via SQL:

- [x] Tickets per Technician
- [x] Average Resolution Time
- [x] Ticket Volume by Date
- [x] Issue Type Breakdown

### 🟨 Power BI
- Dashboards built on cloud SQL source
- Includes custom DAX KPIs, slicers, trend analysis, and visuals

---

## 📊 Power BI Dashboard Highlights

| Visual Type              | Description                                           |
|--------------------------|-------------------------------------------------------|
| KPI Cards                | Total Tickets, Avg Resolution Time, % Resolved Fast   |
| Line & Combo Chart       | Daily ticket volume vs resolution time                |
| Matrix (Heatmap)         | Issue types by day of the week                        |
| Treemap                  | Technician + issue breakdown                          |
| Table                    | Top 5 longest resolution tickets                      |
| Slicers                  | Technician, Month, Issue Type                         |

📍 The dashboard is connected to Azure SQL with scheduled refresh.

---

## 🧠 Technologies Used

- Azure Blob Storage
- Azure Data Factory (Linked Services, Pipelines)
- Azure SQL Database
- Power BI Desktop + Power BI Service
- DAX, SQL, ETL Mapping
- GitHub for code + documentation

---


## 👤 Author

**Wasay Khan**  
📍 Mississauga, ON | 🇺🇸/🇨🇦 | BSc Computer Science  
🔗 [LinkedIn](https://www.linkedin.com/in/abdulwasay-khan)

---
