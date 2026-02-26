# 💄 Rougir Cosmetics – Production Optimization (Linear Programming)

Linear programming model developed to determine the optimal production and outsourcing strategy for Rougir Cosmetics International (RCI).

**Objective:** Minimize total production cost while meeting product demand, labor capacity, and raw material constraints.

---

## 📌 Business Problem

RCI produces three flagship products:

- Face Cream  
- Body Cream  
- Hand Cream  

Due to limited labor hours and raw materials, the firm must decide:

- How much to produce in-house (across two shifts)
- How much to outsource
- How to allocate constrained resources efficiently

Outsourcing costs:
- Face Cream: $40/unit  
- Body Cream: $55/unit  
- Hand Cream: Not allowed  

---

## 📊 Model Overview

### 🎯 Objective Function

Minimize:

Total In-House Production Cost + Outsourcing Cost

Costs include:
- Labor (Stage 1 & Stage 2, two shifts)
- Raw materials (Water, Oil, Scents & Colors, Emulsifiers)
- Outsourcing costs

---

### 🔢 Decision Variables

In-house production:
- FS1, FS2, FS12 (Face Cream)
- BS1, BS2, BS12 (Body Cream)
- HS1, HS2, HS12 (Hand Cream)

Outsourcing:
- FO (Face Cream)
- BO (Body Cream)

All variables ≥ 0.

---

### 📋 Key Constraints

1️⃣ Demand Satisfaction  
- Face Cream ≥ 12,000  
- Body Cream ≥ 8,000  
- Hand Cream ≥ 18,000  

2️⃣ Labor Capacity (per stage & shift)  
- Stage 1 and Stage 2 cannot exceed available hours  

3️⃣ Material Availability  
- Water ≤ 200,000 lbs  
- Oil ≤ 50,000 lbs  
- Scents & Colors ≤ 7,500 lbs  
- Emulsifiers ≤ 15,000 lbs  

---

## ✅ Optimal Solution

**Minimum Total Cost: $1,368,100**

### Production Plan

- Face Cream: Fully outsourced (12,000 units)
- Body Cream: 1,000 produced in-house (Shift 1), 7,000 outsourced
- Hand Cream: Fully produced in-house (both shifts)

---

## 📊 Sensitivity Analysis

### 🔎 Reduced Costs
- Face Cream (Shift 1) would need a ~$19.60 cost reduction to become viable in-house.
- Variables with reduced cost = 0 are already optimal.

### 💰 Shadow Prices
- Scents & Colors: –$50.96  
  → Each additional pound reduces total cost by ~$51.
- Hand Cream Demand: $47.22  
  → Increasing demand increases total cost within allowable range.

---

## 💡 Key Insights

- Face Cream outsourcing is optimal due to labor/material bottlenecks.
- Body Cream is cheaper in-house but capacity limits force partial outsourcing.
- Hand Cream efficiently utilizes both shifts.
- Scents & Colors is a binding constraint and most valuable raw material.
- Water and Oil have slack and may be overstocked.

---

## 🚀 Managerial Recommendations

- Increase availability of Scents & Colors.
- Maintain outsourcing for Face Cream unless labor/material constraints improve.
- Prioritize in-house Body Cream production when feasible.
- Evaluate shift structure for better long-term capacity planning.

---

## 🛠 Tools Used

- Linear Programming (LP)
- Excel Solver
- Sensitivity Analysis (Reduced Cost & Shadow Price Interpretation)

---

## 🎯 Skills Demonstrated

- Linear Programming Formulation  
- Cost Minimization Modeling  
- Production Scheduling  
- Resource Allocation Optimization  
- Sensitivity & Dual Analysis  
- Managerial Interpretation of LP Results  

---

This project demonstrates practical application of optimization modeling to real production and outsourcing decisions under operational constraints.
