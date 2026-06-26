# DecodeLabs Data Science Project 1
## Advanced EDA & Feature Engineering 

### Project Overview
An end-to-end enterprise-grade data science 
pipeline applied to a 1,200-row e-commerce 
dataset as part of the DecodeLabs 
Industrial Training Program (Batch 2026).

### Business Problem
Transform raw, chaotic e-commerce data into 
a mathematically clean dataset ready for 
machine learning algorithms.

### Dataset
- Rows    : 1,200
- Columns : 14
- Domain  : E-commerce Orders

### Pipeline Steps
- ✅ Exploratory Data Analysis (EDA)
- ✅ Missing Value Treatment (Business Logic)
- ✅ Outlier Detection (IQR vs Z-Score)
- ✅ Outlier Treatment (Winsorization)
- ✅ Feature Engineering (3 new features)
- ✅ One-Hot Encoding
- ✅ Multicollinearity Check
- ✅ Pandera Schema Validation

### Key Decisions
- CouponCode NaN treated as NO_COUPON 
  (business logic over statistical imputation)
- IQR chosen over Z-Score 
  (more robust for skewed distributions)
- Winsorization over Deletion 
  (preserves row count)
- drop_first=True 
  (eliminates dummy variable trap)

### Engineered Features
- Discount_Indicator  
  (did customer use a coupon?)
- Order_Completed     
  (was order delivered?)
- Is_Digital_Channel  
  (did customer come from digital channel?)

### Tools & Libraries
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Pandera
- Feast

### Author
Rahma | DecodeLabs Data Science Intern
Batch 2026
