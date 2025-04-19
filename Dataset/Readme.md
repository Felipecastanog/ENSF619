# 📁 dataset

This folder contains the **synthetic dataset** used throughout the project titled  
**"Comparative Analysis of ChatGPT and DeepSeek for Privacy-Preserving Code Generation using Differential Privacy."**

## 📄 Contents

- `Original_Dataset.csv`:  
  A synthetic dataset simulating real-world records from the Calgary Drop-In Centre. It includes **15,991 records** and **28 columns**, representing structured information such as names and dates of birth. The dataset is anonymized and suitable for testing privacy-preserving techniques without compromising individual privacy.

## 🧩 Purpose

The dataset serves as the **input for differentially private code generation and testing**, enabling:
- Evaluation of privacy-preserving mechanisms like the **Laplace mechanism**.
- Comparison of LLM-generated code under identical conditions.
- Simulation of demographic analysis by **birth decade** using tabular data.

This dataset is specifically crafted to mirror the format and complexity of real shelter data while ensuring **no personally identifiable information** is present. It is intended for research and development in **Differential Privacy**, **LLM-assisted code generation**, and **privacy-preserving data analytics**.

## 📌 Usage Notes

- This dataset is used in conjunction with scripts located in the [`codes`](../Codes) folder.
- It should be loaded using `pandas`, cleaned, and filtered before applying DP mechanisms.
- The main DP task in this project is to **count individuals per birth decade** and apply noise to protect privacy.


