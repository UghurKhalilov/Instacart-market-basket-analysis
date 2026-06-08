# Instacart Market Basket Analysis
# Instacart Market Basket Analysis

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Pandas](https://img.shields.io/badge/Pandas-2.x-150458)
![License](https://img.shields.io/badge/License-Apache%202.0-green)

## Overview
This project performs an end-to-end exploratory data analysis (EDA) 
on the Instacart Online Grocery dataset, which contains over 3 million 
orders from 200,000+ anonymous customers. The goal is to uncover 
meaningful patterns in customer purchasing behavior, product popularity, 
and reorder tendencies.

## Dataset
The dataset consists of 5 relational tables:

| Table | Description |
|---|---|
| `orders` | Order-level data including timing and customer info |
| `products` | Product names and IDs |
| `departments` | Department categories |
| `aisles` | Aisle categories |
| `order_products` | Product-level data within each order |

## Project Structure
instacart-market-basket-analysis/
│
├── Pandas_Project_Ughur_Khalilov.ipynb   # Main analysis notebook
└── README.md
## Analysis Summary

### Data Cleaning
- Identified and removed 15 duplicate records from the orders table
- Handled 28,817 missing values in `days_since_prior_order` 
  (first-order customers have no prior order by definition)
- Filled 836 missing values in `add_to_cart_order` with 999
- Standardized product names to lowercase

### Exploratory Data Analysis
| Section | Key Finding |
|---|---|
| Shopping hours | Peak activity between 10:00–16:00 |
| Shopping days | Sunday and Monday are the busiest days |
| Reorder cycle | Most customers reorder on a 7-day cycle |
| Items per order | Typical basket contains 5–10 items |
| Top reordered items | Fresh produce dominates repeat purchases |
| First cart item | Bananas ranked #1 with 15,000+ instances |

## Tools & Libraries
- **Python 3.x**
- **Pandas** — data manipulation and analysis
- **NumPy** — numerical operations
- **Matplotlib** — data visualization

## How to Run
1. Clone the repository
```bash
git clone https://github.com/UghurKhalilov/instacart-market-basket-analysis.git
```
2. Open the notebook
```bash
jupyter notebook Pandas_Project_Ughur_Khalilov.ipynb
```

## License
This project is licensed under the Apache License 2.0 — see the 
[LICENSE](LICENSE) file for details.
