# 📁 prompt

This folder contains the finalized and structured **prompt** used to evaluate and compare Large Language Models (LLMs) — specifically **ChatGPT (GPT-4o)** and **DeepSeek-V3** — for automated code generation in privacy-preserving applications using **Differential Privacy (DP)**.

## 📄 Contents

- `prompt.md`:  
  The complete, step-by-step prompt designed to generate Python code that applies the Laplace mechanism to count records by birth decade in a synthetic dataset.

## 🧩 Purpose

The prompt in this folder is the result of an **iterative prompt engineering process**, which aimed to:
- Maximize code quality and reproducibility.
- Reduce ambiguity and variability in LLM outputs.
- Ensure strict adherence to Differential Privacy principles (ε = 0.1, sensitivity = 1).
- Generate **complete, executable Python scripts** directly from LLM responses.

The final prompt is structured as a **numbered list of explicit tasks**, which proved to be the most effective format for eliciting consistent and correct outputs from both LLMs.

## 🛠 Prompt Design Strategies Explored

During development, several strategies were evaluated and refined:
- ✅ **Structured step-by-step prompting** (most effective)  
- ❌ Goal-oriented prompting (too abstract)  
- ❌ Few-shot prompting (overfitting to example code)  
- ❌ Minimal prompting (ambiguous)  
- ❌ Narrative-style prompting (lack of determinism)

The selected prompt design ensures that LLMs receive **clear instructions**, including file paths, column names, DP parameters, and expected output formatting.

## 🚀 How to Use

You can copy and paste the contents of `final_structured_prompt.txt` into the interface of any general-purpose LLM with code generation capabilities (e.g., ChatGPT, DeepSeek). Modify file paths and column names as needed to adapt to new datasets.

---

This folder is essential for **reproducibility** and helps benchmark LLM behavior in response to a consistent technical query related to Differential Privacy.

