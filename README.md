# 🍽️ Kitchen Pooling Cost Model

A flexible and scalable cost estimation and analysis toolkit for shared kitchen pooling systems — suitable for **apartment communities**, **co-living spaces**, **hostels**, and more. The project helps estimate and analyze food service costs for different group sizes and service tiers using realistic assumptions and scaling models.

---

## 📦 Project Files

| File Name                       | Description |
|--------------------------------|-------------|
| `kitchen_pooling_model.ipynb`     | Main Jupyter Notebook for calculating per-day meal cost estimates across multiple tiers (Ultra Light to Ultra Premium) for group sizes ranging from 1 to 500. |
| `kitchen_pooling_model.csv`       | Output file containing calculated costs for all group sizes and models, including detailed category breakdowns, average costs, and taxes. |
| `eda_kitchen_pooling_model.ipynb` | Notebook containing visual and statistical **Exploratory Data Analysis (EDA)** to better understand cost drivers, trends, and scalability across tiers. |

---

## 🎯 Features

- **Five service tiers**:  
  `Ultra_Light`, `Light`, `Basic`, `Premium`, `Ultra_Premium`
  
- **Cost breakdowns** for:
  - Meals: `Breakfast`, `Lunch`, `Dinner`, `Snacks`, `Tea/Coffee/Milk`
  - Services: `Staff`, `Fuel`, `Packing`, `Delivery`, `Overhead`

- **Scaling logic**:
  - Linear for food items (per person)
  - Sub-linear for shared services (economies of scale)

- **Financial calculations**:
  - `Total Cost`
  - `VAT (5%)`
  - `Grand Total`
  - `Average Cost per Person`

- **CSV Output**:
  - Clean, tabular format for further analysis or dashboarding

---

## 📊 EDA Overview

The EDA notebook (`eda_kitchen_pooling_model.ipynb`) includes:

- **Line plots** for total and average cost vs people count
- **Bar charts** comparing cost components across tiers
- **Pie charts** showing per-category distribution
- **Correlation heatmaps** for category relationships
- **Model comparison visuals**

---

## 💡 Use Cases

- Apartment meal pooling initiatives
- Shared or co-living kitchens
- Budget food planning for hostels, PGs
- Community kitchens / NGOs
- Senior citizen housing with meal services
---

## 🚀 How to Use

### 1. Generate the Cost Model

```bash
jupyter notebook kitchen_pooling_model.ipynb
