# Innomatics Research Labs | Advanced GenAI Internship | Entrance Test

## 📋 Project Overview
This repository contains the complete solution for the Innomatics Research Labs Advanced GenAI Internship Entrance Test, including data integration, analysis, and answers to 25 mandatory questions.

**Date:** 31st January, 2026  
**Test Duration:** 11:00 AM - 6:00 PM  
**Total Questions:** 25 (MCQ + Numerical + Fill in the Blank)

---

## 📁 Files Included

### Data Files
- **orders.csv** - Transactional data containing 10,000 food orders
- **users.json** - User master data with 3,000 user profiles
- **restaurants.sql** - Restaurant master data in SQL format with 500 restaurants

### Notebook & Analysis
- **Innomatics_Entrance_Test.ipynb** - Complete Jupyter notebook with all analysis, code, and answers
- **final_food_delivery_dataset.csv** - Merged dataset (10,000 rows × 16 columns) created from the above three sources

### Documentation
- **ANSWER_SUMMARY.txt** - Comprehensive summary of all 25 answers
- **README.md** - This file

---

## 🔄 Data Integration Process

The solution involves merging three datasets using Pandas:

```
orders.csv (10,000 orders)
    ↓ LEFT JOIN on user_id
users.json (3,000 users)
    ↓ LEFT JOIN on restaurant_id
restaurants.sql (500 restaurants)
    ↓
Final Dataset (10,000 rows with complete information)
```

### Merge Keys
- **Orders ↔ Users:** `user_id`
- **Orders ↔ Restaurants:** `restaurant_id`
- **Join Type:** LEFT JOIN (retains all orders)

---

## 📊 Final Dataset Structure

**Dimensions:** 10,000 rows × 16 columns

**Columns:**
1. `order_id` - Unique order identifier
2. `user_id` - User identifier
3. `restaurant_id` - Restaurant identifier
4. `order_date` - Order date (DD-MM-YYYY)
5. `total_amount` - Order amount in ₹
6. `year`, `month`, `quarter`, `day_of_week` - Temporal features
7. `name` - User name
8. `city` - User city (Bangalore, Chennai, Pune, Hyderabad)
9. `membership` - Membership type (Gold/Regular)
10. `restaurant_name_restaurant` - Restaurant name
11. `cuisine` - Food type (Indian, Chinese, Italian, Mexican)
12. `rating` - Restaurant rating (float 3.0-5.0)

---

## ✅ Answer Summary

### MCQ Answers (Questions 1-10)
| Q# | Question | Answer |
|----|----------|--------|
| 1 | City with highest revenue from Gold members | **Chennai** |
| 2 | Cuisine with highest avg order value | **Mexican** |
| 3 | Distinct users with orders > ₹1000 | **> 2000 category** (2544 users) |
| 4 | Rating range with highest revenue | **4.6 – 5.0** |
| 5 | City with highest avg value for Gold members | **Chennai** |
| 6 | Cuisine with lowest restaurants but high revenue | **Chinese** |
| 7 | % of orders by Gold members | **50%** |
| 8 | Restaurant with highest avg value (< 20 orders) | **Restaurant_294** |
| 9 | Membership + Cuisine with highest revenue | **Regular + Mexican** |
| 10 | Quarter with highest revenue | **Q3 (Jul–Sep)** |

### Numerical Answers (Questions 11-16)
| Q# | Question | Answer |
|----|----------|--------|
| 11 | Total Gold member orders | **4987** |
| 12 | Total Hyderabad revenue (rounded) | **1889367** |
| 13 | Distinct users with at least 1 order | **2883** |
| 14 | Avg order value for Gold members | **797.15** |
| 15 | Orders from restaurants with rating ≥ 4.5 | **3374** |
| 16 | Orders in top revenue city for Gold members | **1337** |

### Fill in the Blanks (Questions 17-25)
| Q# | Answer |
|----|--------|
| 17 | **user_id** |
| 18 | **SQL** |
| 19 | **10000** |
| 20 | **NaN (null)** |
| 21 | **merge()** |
| 22 | **users.json** |
| 23 | **restaurant_id** |
| 24 | **cuisine** |
| 25 | **multiple times (per order count)** |

---

## 📈 Key Statistics

### Revenue Breakdown
- **Total Revenue:** ₹8,011,624.12
- **Average Order Value:** ₹801.16
- **Median Order Value:** ₹806.30

### Geographic Distribution
1. Bangalore: ₹2,206,946.58 (27.5%)
2. Chennai: ₹1,990,513.03 (24.8%)
3. Pune: ₹1,924,797.93 (24.0%)
4. Hyderabad: ₹1,889,366.58 (23.6%)

### Cuisine Distribution
- Mexican: 2,581 orders (₹808.02 avg)
- Italian: 2,532 orders (₹799.45 avg)
- Indian: 2,469 orders (₹798.47 avg)
- Chinese: 2,418 orders (₹798.39 avg)

### Membership Distribution
- Gold Members: 4,987 orders (49.9%)
- Regular Members: 5,013 orders (50.1%)

---

## 🛠️ Technology Stack

- **Python 3.12**
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computations
- **Jupyter Notebook** - Interactive analysis

---

## 💻 Notebook Execution

The Jupyter notebook includes:
1. ✓ Library imports and environment setup
2. ✓ Loading all three datasets
3. ✓ Data preprocessing and cleaning
4. ✓ Merging datasets with proper joins
5. ✓ MCQ analysis (Questions 1-10)
6. ✓ Numerical calculations (Questions 11-16)
7. ✓ Fill-in-the-blanks answers (Questions 17-25)
8. ✓ Summary statistics and insights
9. ✓ Comprehensive code comments

### To Run the Notebook:
```bash
jupyter notebook Innomatics_Entrance_Test.ipynb
```

---

## 📝 Code Quality

- ✓ All code properly commented
- ✓ Clear variable naming conventions
- ✓ Step-by-step data processing
- ✓ Verification of results
- ✓ Reproducible analysis

---

## 🎯 Key Insights

1. **User Spending:** 88.2% of users have spent more than ₹1000
2. **Revenue Peak:** Q3 (July-September) generates the highest revenue
3. **Geographic Leader:** Bangalore leads in revenue generation
4. **Membership Impact:** Nearly equal distribution with Gold members spending slightly more per order in Chennai
5. **Quality Effect:** High-rated restaurants (4.6-5.0) generate maximum revenue
6. **Cuisine Efficiency:** Mexican cuisine achieves highest average order value despite having only 120 distinct restaurants

---

## ✨ Features

- Complete data integration from multiple formats (CSV, JSON, SQL)
- Thorough exploratory data analysis
- Statistical insights and trend analysis
- Comprehensive answer documentation
- Ready-to-submit Jupyter notebook

---

## 📞 Contact Information

**Test Date:** 31st January, 2026  
**Participant Email:** shrushtisakat2023.ainds@mmcoe.edu.in

---

## 📌 Important Notes

- The final merged dataset is the single source of truth for all analysis
- All left joins preserve all orders from the transactional data
- Results have been verified and rounded as per question requirements
- Code is production-ready and fully documented

---

**Status:** ✅ Complete and Ready for Submission

Generated: January 31, 2026
