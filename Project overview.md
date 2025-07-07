# Market Basket Analysis & Cross-Selling Recommendations

## Objective
Identify products frequently purchased together and discover cross-selling opportunities using association rule techniques.

---

## Dataset
**Retail Product Transaction Dataset**
- **Records:** 30,000 transactions
- **Fields:**
  - Transaction ID
  - Customer ID
  - List of purchased products
  - Transaction timestamp
- **Unique Products:** 38

---

## Tools & Technologies
- **Python:** pandas, mlxtend
- **Power BI:** interactive visualizations and dashboards

---
    
1. **Data Preprocessing**
   - Parsed and cleaned product lists into a binary matrix.
   - Converted purchase indicators to boolean format.
   - Prepared basket representation for analysis.

2. **Frequent Itemset Mining**
   - Applied the **Apriori Algorithm** to identify frequent combinations.
   - Minimum support threshold: **2%**.

3. **Association Rule Generation**
   - Calculated rules with:
     - Support
     - Confidence
     - Lift
   - Filtered for strong and relevant associations.

4. **Data Cleaning**
   - Converted frozenset outputs to clean product names.
   - Exported cleaned datasets for visualization.

---

## Visualizations (Power BI)
- **Table of Top Association Rules**  
  Displays antecedents, consequents, support, confidence, and lift.
- **Matrix Heatmap**  
  Visualizes confidence between each product pair.
- **Bar Chart of Most Frequent Antecedents**  
  Highlights products most often acting as rule triggers.
- **Treemap & Bar Chart of Single Product Frequency**  
  Shows overall product popularity.
- **KPI Cards**
  - Total number of rules
  - Maximum lift
  - Maximum confidence
- **Slicers**
  - Interactive filtering by confidence and lift

---

## Key Insights
- **Milk → Cereal** emerged as the strongest association (lift: **2.5**, confidence: **58%**).
- Several product pairs demonstrated strong co-purchase behavior.


- **Top Rules Table:** Interactive view of rules with support, confidence, and lift.
- **Confidence Matrix:** Visual comparison of antecedent-consequent pairs and strong co-purchase behavior
- **Bar Chart of Most Frequent Antecedents:** Identifies products driving most cross-selling and bundling opportunites.
- **KPI Cards:** 
  - Total Rules Generated: 18
  - with **Milk → Cereal** with  Max Confidence: 58% & Max Lift: 2.51

---

## Recommendations
- Bundle **Milk and Cereal** in promotions to increase basket size.
- Launch targeted marketing campaigns around the top frequent pairs like cheese and cereal.
- Use high-lift rules as input to recommend bundles & cross selling pairs in e-commerce.

