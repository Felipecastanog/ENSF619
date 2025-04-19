I have a CSV file located at this path: `/Users/felipecastanogonzalez/Downloads/ChfSynthData-13_09_2024.csv` 

I want a complete Python script that applies Differential Privacy using the Laplace mechanism on counts by decade of birth. 

Please generate a clean, ready-to-run Python script that performs the following steps: 
1. Loads the dataset using `pandas`.
2. Filters and cleans the data by:
     -Dropping duplicates
     -Removing rows with missing values in: `"FirstName"`, `"LastName"`, `"DobDay"`, `"DobMonth"`, `"DobYear"`
     -Converting `"DobYear"` to integer
4. Keeps only these columns: `"FirstName"`, `"LastName"`, `"DobDay"`, `"DobMonth"`, `"DobYear"`
5. Creates a new column `"Decade"` from `"DobYear"` by flooring it to the nearest multiple of 10 (e.g., 1985 → 1980).
6. Counts the number of records in each decade (`true_counts`).
7. Applies the **Laplace mechanism** (from `diffprivlib`) with `epsilon = 0.1` and `sensitivity = 1` to each decade count.
8. Produces a `DataFrame` that compares true counts vs differentially private counts by decade.
9. Prints the resulting comparison table.

Please include: 
  -All necessary imports (`pandas`, `numpy`, `diffprivlib.mechanisms.Laplace`) 
  -Clear code structure with step comments 
  -`max(0, ...)` to prevent negative counts 
  -Output printed as a clean comparison table using `to_string(index=False)` 
  
Do not use placeholders. Use the exact path and column names I provided.
