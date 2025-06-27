# 📊 Interactive Power BI Dashboard – Headcount Analysis

This project showcases a dynamic and **interactive** Power BI dashboard that visualizes headcount data across multiple vendors, rooms, and regions in Korea. The dashboard was created to replace an outdated, table-based system that required manually opening separate dashboards for each month to observe trends.

---

## 🧩 Problem Statement

At work, a team was relying on an old, inefficient dashboard that displayed headcount data in a compact and static table format. It was difficult to navigate, hard to read, and required users to open a separate dashboard file for each month in order to view trends. It lacked both interactivity and visual clarity.

To improve this, I developed an interactive Power BI dashboard that:
- Consolidates all months into a single view
- Allows dynamic filtering by vendor, room, and month
- Displays trends and insights through clean, informative visuals
- Significantly enhances user experience and decision-making

---

## ✅ Features

- 🎯 **Dynamic Filtering**
  - Filter by **vendor** — the vendor logo updates accordingly
  - Filter by **room** and **year/month**
- 📈 **Key Metrics (update dynamically based on filters)**
  - Total Headcount (HC)
  - Full-time HC
  - Hybrid HC
  - Month-over-month (MoM) changes for each
- 📊 **Visuals**
  - **Line chart**: Full-time vs. Hybrid headcount trends over time  
    *(not affected by the Year/Month filter to show full context)*
  - **Donut chart**: Headcount breakdown by room  
    *(not affected by room filter for consistent comparison)*
  - **Bar chart**: Line of Business (LOB) headcount, filtered by vendor, room, and month
  - **Map of Korea**: Bubble size shows headcount per room by city location

---

## 🌍 Technologies Used

- Power BI
- DAX
- Power Query
- Geographic mapping (Map visual)
- Custom visual formatting and conditional logic

---

## 🧮 Data Structuring for Power BI

To make the data model usable and efficient in Power BI, I designed the dataset in a **flat, tabular structure** ideal for analysis and filtering. Key design decisions include:

- **No merged cells or nested structures** — each row represents a unique data point (granular to vendor, room, LOB, month, and employee type).
- Created a **`YearMonth`** column for simplified time-based filtering and a separate **`Date`** column to support Power BI's time intelligence functions.
- Included **dimension fields**:
  - `Vendor`
  - `City`
  - `Room`
  - `EmployeeType`
  - `LineOfBusiness`
- Numeric field `Headcount` is clean and ready for aggregation (sum, average, MoM comparisons).
- Ensured **consistency in categorical naming** (e.g., “Retail Banking”, “IT Support”) to prevent data mismatches or filtering issues.

This structure supports:
- Accurate DAX calculations
- Clean filtering without the need for excessive data transformation
- Easy creation of slicers and visuals based on multiple attributes

![Excel Sheet](https://github.com/ericyang91/Employee_Headcount_Dashboard/blob/main/screenshots/s2.JPG)

> 📌 The data shown in this project is anonymized and generated solely for demonstration purposes.

---

## 🔗 Other

> 🚨 *Data is anonymized and synthetic for demonstration purposes*


---

## 📷 Screenshots

![Dashboard Preview](https://github.com/ericyang91/Employee_Headcount_Dashboard/blob/main/screenshots/s1.JPG)

---

## 📌 Key Impact

- 🧠 Improved insight generation by visualizing headcount trends in a single view
- ⏱️ Reduced time spent switching between multiple dashboard files
- 💡 Enabled filtering by vendor, location, and month to support better decision-making
- 📍 Introduced geographic context and visual clarity using maps and charts

---

## 🧑‍💻 Author

**Ji Yeol Yang**  
Aspiring Data Analyst with a passion for clean data visualization and storytelling through analytics

🔗 [GitHub Profile](https://github.com/ericyang91)  
📧 [Email me](mailto:ericjyyang@gmail.com)

---

