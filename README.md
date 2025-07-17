# Data Cleaning Automation Script

This project automates the process of cleaning product listing data to prepare it for annotation and client handoff. It is especially useful for time-saving and quality control in high-volume environments.

## 💡 Features

- Removes unreadable WPIDs  
- Filters out entries with explicit content  
- Cleans double quotes from URLs  
- Removes duplicate entries (retaining the first)  
- Rearranges rows based on user-defined keywords (e.g., "Shirt", "Trouser")  
- Organizes removed data into separate CSVs for audit and client reporting  

## 🧾 Files

- `clean_and_sort_products.py`: Standalone Python script for automation  
- `Seed_Data_Cleaner_Refactored.ipynb`: Jupyter notebook version for step-by-step explanation and editing  

## 📥 Input Format

The script expects a CSV with the following columns:  
`WPID,Item ID,Product Name,Image URL1,Image URL2,Image URL3`

## ⚙️ How to Use

### Option 1: Run the Script (`.py`)

```bash
python clean_and_sort_products.py
```

Before running, open the script and update:

- `input_filename` (your input CSV file name)  
- `output_filename` (desired output file name)  
- `explicit_words` (list of explicit words to remove)  
- `sort_keywords` (the keywords used to group similar product types)  

### Option 2: Use the Notebook (`.ipynb`)

Open `Seed_Data_Cleaner_Refactored.ipynb` in Jupyter or Google Colab to see the code step-by-step and make edits easily.

## 📊 Output

- `Cleaned_Data.csv` – Final cleaned and organized data  
- `Removed_Explicit.csv` – Rows with explicit content  
- `Removed_Unreadable.csv` – Rows with invalid WPIDs  
- `Removed_Duplicates.csv` – Duplicate entries (first kept)  

## 👤 Author

Daisy Ch — Data Analyst & Operations Automation Specialist
