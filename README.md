# Healthcare-Anlaytics-Dashboard 🚑📊
Focuses on COVID data in the US from 2020 - 2024

**📌 Project Overview**

This project focuses on analyzing and forecasting hospital resource utilization in the United States using real-world COVID-19 hospital capacity data. The dashboard provides actionable insights into inpatient bed usage, ICU utilization, and staffing shortages, helping healthcare organizations optimize resources and plan for surges in demand.

**🎯 Objectives**

- Clean and transform raw hospital capacity data for analysis.
- Build an interactive Power BI dashboard to visualize utilization trends.
- Apply time-series forecasting models (DeepAR in AWS SageMaker, PyTorch Forecasting) to predict hospital demand.
- Experiment with synthetic data generation (GANs) for small-scale test cases.
- Deliver a decision-support tool for hospital administrators and policymakers.

**🗂️ Dataset**

- Source: COVID-19 Hospital Capacity Dataset (HHS/CDC).
- Key Columns Used:
  - inpatient_bed_utilization
  - icu_bed_utilization
  - critical_staffing_shortage_today_yes
- Data was preprocessed in MySQL Workbench, with nulls and zero-value rows cleaned before visualization and forecasting.

**🔧 Tech Stack**

- Data Cleaning & SQL: MySQL Workbench
- Visualization: Power BI (interactive dashboards, maps, DAX formulas)
- Forecasting:
  - AWS SageMaker (DeepAR for time-aware forecasting)
  - PyTorch Forecasting (local experimentation with ARIMA/Prophet alternatives)
  - Optional: Generative Adversarial Networks (GANs) for synthetic data augmentation

**📊 Dashboard Features**

- ICU Utilization Heat Map: State-wise visualization of ICU occupancy.
- Staffing Shortage Trends: Line charts tracking shortage percentages over time.
- National Aggregates: Daily averages across all states for quick benchmarking.
- Calculated Metrics: Bed usage rates, total hospital counts, and conditional formatting for critical thresholds.

**🤖 Forecasting Approach**

- DeepAR (SageMaker): Trained on time-series data to predict utilization trends.
- PyTorch Forecasting: Local experimentation with alternative forecasting methods.
- GANs (optional): Synthetic dataset generation for controlled experiments.
