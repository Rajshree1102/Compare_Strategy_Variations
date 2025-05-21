# Compare Strategy Variations

## 🔍 Project Overview  
This Power BI dashboard allows users to compare the performance of two trading strategy variations side by side. The analysis focuses on PnL (Profit and Loss), with dynamic selection of strategy and variation for each comparison panel. It uses four separate CSV files, each representing a unique combination of strategy and variation.  

## 📁 Source Files  
The following CSV files are used in this project:  
strategy_1_var_1.csv  
strategy_1_var_2.csv  
strategy_2_var_1.csv  
strategy_2_var_2.csv  

## 🧩 Data Modeling Steps  
### Import Data  
Load all four CSV files into Power BI as separate tables.  

### Create Variation Selector Table  
Append all four tables in Power Query to create a master selector table with unique combinations of strategy and variation.  
Remove duplicates and load as SelectorTable.  

### Create Two Slicer Panels (A & B)  
Use SelectorTable to build two slicer sets:  
Slicer 1A & 1B: Select Strategy  
Slicer 2A & 2B: Show Variations filtered by selected Strategy  

### Model Relationships  
No relationships needed between the tables since they remain independent and are filtered separately.

![Alt text](C:/Users/khush/OneDrive/Desktop/OneDrive/Pictures/Screenshots/Screenshot 2025-05-21 155225.png)
