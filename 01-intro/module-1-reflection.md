
# 📘 Module 1: Introduction to MLOps – Reflection & Summary

## 1. ✅ What was covered?
- Overview of **MLOps** and its role in bridging ML development and production.
- Understanding the **MLOps maturity model** and the evolution from manual processes to automated pipelines.
- Introduction to the **NYC Yellow Taxi dataset** (used as a running example throughout the course).
- Setting up the **project environment** and working with tools like:
  - `pandas` for data analysis
  - `pyarrow` for working with Parquet files
- Writing utility functions to:
  - Read and preprocess Parquet data
  - Filter outliers in ride durations
  - Convert categorical features to string format

## 2. 🧠 What did I already know, and what was new?

**Already knew:**
- How to work with `pandas`, `read_parquet`, and basic data cleaning.
- Using Python functions to modularize data preprocessing steps.

**New concepts:**
- The **MLOps maturity model** (manual → automated → CI/CD).
- The rationale for MLOps in real-world ML workflows.

## 3. ❓ What was challenging or confusing?

- Understanding why **'PULocationID', 'DOLocationID'** are categorical data was tricky at first :).
- The subtle differences between CSV and Parquet formats when loading data and handling timestamps.
- Understanding One-Hot Encoding and its implications for categorical features.

## 4. 👨‍🏫 How would I explain this to a junior colleague?

> “MLOps is all about operationalizing machine learning. In this module, we used the NYC Taxi dataset to explore what a typical raw ML dataset looks like and how to clean it. We wrote a function that:
> 1. Loads the data from either CSV or Parquet,
> 3. Calculates trip duration,
> 4. Removes outliers, and
> 5. Prepares features like pickup/dropoff locations.
> 
> This kind of preprocessing is the foundation for building robust ML workflows.”

## 5. 🛠️ Which tools or workflows would I apply in a real project?

- **Reusable Data Loaders**: Creating generalized functions like `read_dataframe()` for consistent data preprocessing.
- **Format Agnostic Readers**: Supporting both `.csv` and `.parquet` in production ingestion pipelines.
