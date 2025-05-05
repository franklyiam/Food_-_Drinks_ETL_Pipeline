# 🍔 Food & Drink ETL Pipeline

This project is an ETL (Extract, Transform, Load) pipeline designed to clean and transform mobile app data from the Food & Drink category. It reads the dataset, formats and standardizes key columns, and filters incomplete data, preparing it for analysis and visualization.

---

## 📁 Project Structure

```
Food_Drink_ETL/
├── Food_Drink.csv               # Raw dataset
├── Food_Drink_ETL_Code.ipynb    # Main ETL code (Jupyter Notebook)
├── transformed_data.csv         # Output CSV after transformation (generated)
├── log_file.txt                 # Optional: ETL logs (generated)
├── README.md                    # You're here!
```

---

## 🛠 Requirements

Ensure you have the following installed:

- Python 3.7+
- Jupyter Notebook (or Jupyter Lab)
- pandas
- plotly

You can install the required libraries via pip:

```bash
pip install pandas plotly
```

---

## 🚀 How to Run the Code

### 1. **Download the Files**
Ensure `Food_Drink.csv` and `Food_Drink_ETL_Code.ipynb` are in the same local directory.

### 2. **Open the Jupyter Notebook**
Launch the notebook in your terminal or IDE:

```bash
jupyter notebook Food_Drink_ETL_Code.ipynb
```

### 3. **Update the File Paths**
In the notebook, replace any Google Colab-specific paths like:

```python
'/content/drive/MyDrive/Colab Notebooks/Food_Drink.csv'
```

with a relative or absolute path to your local file, e.g.:

```python
'Food_Drink.csv'
```

Similarly, update any output file paths (e.g., `log_file.txt`, `transformed_data.csv`) to local paths.

### 4. **Run the Notebook**
Step through each cell in order. The ETL pipeline will:
- Extract the raw data
- Clean and transform values in columns like `Reviews` and `Downloads`
- Remove records missing critical data (`Star Rating`, `Reviews`)
- Save the cleaned dataset as `transformed_data.csv`

---

## 🧪 Testing & Validation

- **Preview the transformed dataset:** Use `df.head()` or open `transformed_data.csv` in any CSV viewer.
- **Use visualizations:** The notebook includes a Plotly bubble chart to visualize trends in star ratings, reviews, downloads, and categories.

---

## 📌 Notes

- The transformation logic handles units like `K`, `M`, `L`, `Cr`, and `B` and formats the numbers cleanly.
- The pipeline drops rows where `Star Rating` or `Reviews` are empty or invalid.

---

## 📧 Support

If you run into any issues, feel free to reach out to Byte & Beyond Group

Happy ETL-ing! 🎉
