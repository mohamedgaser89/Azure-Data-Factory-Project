# Azure-Data-Factory-Project
Azure Data Factory Project - Data Flow Pipeline
# Azure Data Factory Project - Data Flow Pipeline

## 📌 Overview

This project demonstrates building a data pipeline using **Azure Data Factory** to process and transform CSV data.

The pipeline reads data from a source file, applies transformations, and writes the cleaned data to a sink.

---

## 🛠️ Technologies Used

* Microsoft Azure Data Factory
* Data Flow
* CSV (Delimited Text)
* Azure Integration Runtime

---

## 🔄 Pipeline Workflow

### 1. Source

* Reads data from a CSV file (DelimitedText1)
* Input contains columns such as:

  * order_id
  * order_date
  * customer_id
  * product
  * category
  * quantity
  * unit_price

---

### 2. Select Transformation

* Renames and selects required columns
* Removes unnecessary fields

---

### 3. Derived Column

* Creates or updates columns
* Example transformations:

  * Cleaning `order_id`
  * Formatting `order_date`
  * Calculating new values if needed

---

### 4. Sort

* Sorts data based on:

  * `order_id_clean`

---

### 5. Sink

* Writes processed data back to a CSV file

---

## ⚙️ Pipeline Configuration

* Integration Runtime: AutoResolveIntegrationRuntime
* Compute Size: Small
* Logging Level: Verbose

---

## ▶️ How to Run

1. Open Azure Data Factory
2. Go to the pipeline (`pipeline1`)
3. Click **Debug** or **Trigger**
4. Monitor execution in the **Monitor** tab

---

## 📂 Project Structure

* `pipeline1` → Main pipeline
* `dataflow1` → Data transformation flow
* `dataset` → CSV source and sink configuration

---

## 📊 Output

Cleaned and transformed CSV file ready for analysis.

---

## 🚀 Future Improvements

* Add error handling
* Parameterize datasets
* Connect to database instead of CSV
* Schedule pipeline using triggers

---


