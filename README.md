# 📊 E-Commerce Sales Data Analysis  
**A comprehensive dashboard for analyzing sales performance, regional orders, and product insights.**  

---

## 🌟 **Project Overview**  
This Power BI report provides an interactive analysis of e-commerce sales data, focusing on key metrics like revenue, profits, orders, and returns. Designed with a user-friendly interface, it includes dynamic filtering, drill-down capabilities, and visualizations tailored for executive summaries, regional insights, and product performance.  

---

## 📂 **Dataset Used**  
- **Source File**: `Dataset.xlsx`  
- **Tables**:  
  - **Sales**: Contains transaction details (e.g., Order Date, Product ID, City, Revenue).  
  - **Return**: Tracks returned transactions.  

---

## 🛠️ **Tasks Completed**  
### **Data Preparation & Modeling**  
1. **Loaded** "Sales" and "Return" tables into Power BI.  
2. **Created Dimension Tables** from "Sales":  
   - `Date` (Order Date)  
   - `Region` (City)  
   - `Product`, `Product Sub-Category`, `Product Category` (hierarchical structure).  
3. **Built Data Models**:  
   - **Star Schema**: Fact table "Sales" linked to "Date", "Region", and "Return".  
   - **Snowflake Schema**: "Product" tables linked hierarchically to "Sales".  
4. **Calculated Tables in "Sales"**:  
   - `Cost Total` (Product + Shipping Cost)  
   - `Revenue` (Pre-discount price)  
   - `Profit` (Revenue - Cost).  

---

## 📊 **Report Pages Overview**  
### **1. Homepage**  
- **Title**: "E-Commerce Sales Analysis" with a stylized text/shape visual.  
- **Navigation Buttons**: Jump to Executive, Regional Order, or Sales pages.  

### **2. Executive Page**  
- **KPIs**: Total Orders, Quantities, Products, Revenues, Profits.  
- **Visuals**:  
  - Donut Charts (Shipping Modes, Customer Segments).  
  - Profit-by-Continent Column Chart with tooltips.  
  - Product Sub-Category Summary Table.  
  - **Date Slicer** (filters all visuals).  

### **3. Regional Order Page**  
- **Visuals**:  
  - Donut Chart (Order Priorities).  
  - Drill-down Map (Country → State → City) with order quantities and revenues.  
  - Top 5 Cities Bar Chart.  
  - **Continent Slicer**.  

### **4. Sales Page**  
- **KPIs**: Costs, Revenues, Profits (including returned amounts and margin %).  
- **Visuals**:  
  - Monthly Summary Table with Data Bars.  
  - Drill-down Area Chart (Month → Week → Date).  
  - **Product Name Slicer**.  

---

## 🎨 **Features**  
- **Interactive Navigation**: Buttons to switch pages and reset filters.  
- **Dynamic Filtering**: Slicers for dates, continents, and products.  
- **Drill-Down Capabilities**: Explore data hierarchically (e.g., map locations, time periods).  
- **Tooltips**: Additional context for charts (e.g., country/city counts, revenue percentages).  

---

## ⚙️ **How to Use**  
1. **Open the Report**: Launch the `.pbix` file in Power BI Desktop.  
2. **Navigate**: Use buttons on the Homepage to explore pages.  
3. **Filter Data**: Adjust slicers to focus on specific regions, dates, or products.  
4. **Reset Views**: Click the "Default View" button on any page to clear filters.  

---

## 📸 **Screenshots**  
*(Include screenshots of each page here for visual reference)*  

---

## 💡 **Tips**  
- Hover over chart elements to see tooltips.  
- Use the drill-down arrows (↕️) in visuals like the map or area chart for deeper insights.  
- Double-click slicers to reset selections.  

---

## 🙏 **Credits**  
Developed with ❤️ by [Your Name].  
Data sourced from `Dataset.xlsx`.  
