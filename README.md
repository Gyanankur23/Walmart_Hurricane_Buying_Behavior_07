# Walmart_Hurricane_Buying_Behavior_07 CaseCraft Analytics Project 7

## 🌪️ Overview  
This project analyzes Walmart’s consumer purchasing behavior before hurricanes using synthetic transaction data. It focuses on surge detection, category-level trends, and predictive modeling to support inventory and logistics planning.

## 🎯 Objective  
To identify hurricane-prep buying patterns across regions and categories, and build a classification model to predict surge purchases.

## 🛍️ Dataset & Features  
- Dates: Aug–Sep 2023  
- Regions: Florida, Texas, Louisiana  
- Categories: Water, Batteries, Canned Food, Flashlights, Snacks, Clothing, Electronics  
- Features: units_sold, price, revenue, day of year  
- Surge window: Aug 25–30 (Florida only)

## 📈 Visual Explorations  
- Line chart: Daily units sold by category  
- Bar chart: Revenue by region and category  
- Line chart: Surge buying behavior in Florida (Aug 25–30)  
- Bar chart: Surge ratio by category  
- Histogram: Demand elasticity distribution  
- Scatterplot: Inventory vs Revenue

## 🔍 Surge Detection Logic  
- Essentials (Water, Batteries, Canned Food, Flashlights) show 2–4× spike in Florida during surge window  
- Non-essentials remain stable  
- Surge ratio calculated as mean units sold during surge vs pre-surge

## 🤖 Classification Model  
- Target: `is_prep` (binary flag for surge purchase)  
- Features: price, units_sold  
- Model: Random Forest  
- Performance:  
  - Precision: 1.00  
  - Recall: 1.00  
  - F1-score: 1.00  
  - Accuracy: 100%

## 🧠 Key Insights  
1. **Surge Categories**: Water, Batteries, Canned Food, Flashlights dominate pre-hurricane buying  
2. **Regional Impact**: Florida shows highest spike; other regions remain stable  
3. **Temporal Window**: Aug 25–30 is critical for surge detection  
4. **Model Utility**: Classification accurately flags prep purchases using just price and units_sold  
5. **Business Implication**: Enables automated alerts for inventory restocking and logistics coordination

## ✅ Final Conclusion  
Walmart’s hurricane buying behavior reveals predictable surges in essential categories. This project offers a modular framework for surge detection, regional analysis, and predictive modeling—ideal for retail preparedness, supply chain optimization, and emergency response planning.