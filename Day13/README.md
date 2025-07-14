# Day 13 — Linear Regression

**Date:** July 09, 2025

---

## Overview

On **Day 13**, I explored **Linear Regression**, one of the simplest and most important supervised learning algorithms.  
I learned how it maps data points with an optimized linear function to make predictions based on a linear relationship between input and output.

---

## Key Concepts

- **Definition:** Predict a dependent variable (Y) based on an independent variable (X) using a straight line.
- **Assumption:** Output changes at a constant rate with input.
- **Equation:**  
  - *Simple Linear Regression:* `ŷ = θ₀ + θ₁x`
  - *Multiple Linear Regression:* `ŷ = θ₀ + θ₁x₁ + θ₂x₂ + ⋯ + θₙxₙ`

- **Examples:**  
  - Predicting student exam scores based on hours studied.
  - Real Estate Pricing, Financial Forecasting, Agriculture Yield, E-commerce trends.

---

## Types of Linear Regression

- **Simple Linear Regression:** One input feature (Univariate).
- **Multiple Linear Regression:** Multiple input features (Multivariate).

---

## Python Implementation

Key implementation steps:
1️ **Import Libraries:** pandas, numpy, matplotlib.  
2️ **Load Dataset:** Separate training & testing data.  
3️ **Forward Propagation:** Calculate predictions using `Y = mx + c`.  
4️ **Cost Function:** Mean squared error.  
5️ **Backpropagation:** Compute gradients for `m` and `c` and update using learning rate.  
6️ **Train:** Animate the line fitting process and save as a GIF.

---

## Files

- `Day13.pdf` — Full explanation & Python code.

---

> **"Linear Regression draws a straight line through the noise — revealing trends that data hides."**

