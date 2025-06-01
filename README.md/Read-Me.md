# Practical Data Cleaning & Analysis: Spectrum Shades LLC

## 📊 Objective
This project addresses data quality and performance issues at Spectrum Shades LLC, a leading supplier of concrete color solutions. The company has experienced a rise in customer complaints regarding inconsistent product color quality. The goal of this analysis is to clean the production data, investigate the influence of material suppliers and pigment usage on product quality, and provide actionable insights to improve overall customer satisfaction and product reliability.

## 🧪 Dataset
- **File used**: `production_data.csv`
- **Content**: Contains batch production records including pigment type and quantity, mixing parameters, and final product quality scores.

## 🛠️ Tools & Technologies
- Python
- pandas, numpy, scipy
- Jupyter Notebook

## 📂 Project Structure
- `spectrum_shades_quality_analysis.ipynb`: Full notebook with all 4 tasks
- `data/production_data.csv`: Original dataset
- `README.md`: Project description

## ✅ Tasks Summary

### Task 1 – Data Cleaning
- Verified and cleaned `production_data.csv` according to given criteria
- Handled missing values:
  - Replaced missing supplier IDs and pigment types with defaults
  - Imputed missing numerical values with median or mean
- Output: `clean_data` DataFrame with clean and structured production data

### Task 2 – Grouped Aggregation
- Computed average `product_quality_score` and `pigment_quantity` grouped by `raw_material_supplier`
- Output: `aggregated_data` DataFrame

### Task 3 – Conditional Filtering
- Filtered data where:
  - `raw_material_supplier == 2`
  - `pigment_quantity > 35 kg`
- Calculated average `product_quality_score` for this subset
- Output: `pigment_data` DataFrame (1-row)

### Task 4 – Statistical Analysis
- Calculated mean and standard deviation for:
  - `pigment_quantity`
  - `product_quality_score`
- Computed Pearson correlation coefficient between both variables
- Output: `product_quality` DataFrame with 5 columns

## 📈 Key Takeaways
- Supplier type and pigment quantity affect product quality
- Proper cleaning and validation of production data are essential before analysis
- Moderate correlation observed between pigment quantity and quality score (context-dependent)


👤 Created by: Salma Moustaouli  
