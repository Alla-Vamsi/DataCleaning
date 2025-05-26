# DataCleaning

## 🧹 Medical Appointment No-Show Data Cleaning

This repository contains a data cleaning project for the **KaggleV2-May-2016.csv** dataset, which includes medical appointment records and whether patients showed up for their appointments.

### 📁 Dataset Source

The dataset was originally published on [Kaggle](https://www.kaggle.com/datasets/joniarroba/noshowappointments) and includes over 110,000 medical appointments in Brazil.

### 📌 Objective

The goal of this project is to clean and prepare the dataset for analysis by:

* Fixing column names
* Handling missing and duplicate data
* Converting data types
* Standardizing text values
* Formatting dates properly

---

### Cleaning Steps Performed

1. **Renamed Column Headers**

   * Converted all column names to lowercase and removed special characters/spaces.
   * Corrected misspelled columns like `hipertension` → `hypertension`.

2. **Handled Missing Values**

   * Dropped rows with any `NaN` values to ensure data completeness.

3. **Removed Duplicates**

   * Checked for and removed duplicate rows to prevent data distortion.

4. **Standardized Text Values**

   * Ensured gender values are in uppercase (`M`, `F`).
   * Converted `no_show` values to boolean (`True` = No-show, `False` = Showed up).

5. **Converted and Formatted Dates**

   * Converted `scheduledday` and `appointmentday` columns to `dd-mm-yyyy` format.

6. **Corrected Data Types**

   * Ensured `age` is an integer and filtered out negative values.
   * Dates stored as strings in consistent format for readability.

---

### How to Use

1. Run the cleaning script:

   ```bash
   python clean_data.py
   ```

2. Output:

   * Cleaned data will be saved as `Cleaned_Medical-Appointment-No-Show.csv`


