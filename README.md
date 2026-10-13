# Supermarket Sales Analysis

**Author:** Gajanan Harinarayan Raje
**Program:** AICTE | IBM SkillsBuild Data Analytics with AI Internship 2026 (BharatCares)
**Institution:** MGM's College of Computer Science & IT, Nanded (SRTMU University)

## Project Description
A data analytics project on 500 supermarket sales transactions (January to 1 July 2026) from four branches in four cities. The notebook loads the data, checks it for missing or incorrect values, verifies Sales = Quantity x Unit Price, summarises sales with totals, counts and averages, draws charts and ends with business decisions.

## Dataset
- **File:** [`supermarket_sales.csv`](supermarket_sales.csv) (included in this repository), 500 rows and 13 columns
- **Source:** Data provided for the *Supermarket Sales Analysis DA project* in the IBM SkillsBuild Data Analytics with AI internship (Masterclass 4). Project workbook: https://docs.google.com/document/d/1DVCIE1WCNGpbBrVBIfEkqaN6Qw9lJkCS_p-P5zeQV7Q/edit
- **Columns:** Invoice ID, Date, Branch, City, Customer Type, Gender, Product, Category, Quantity, Unit Price, Payment, Rating, Sales

## Technologies Used
- Python 3.9+
- pandas and NumPy for data cleaning and summaries
- Matplotlib and Seaborn for charts
- Jupyter Notebook

## Project Files
| File | Purpose |
|---|---|
| `Gajanan_Raje_SupermarketSalesAnalysis.ipynb` | Complete analysis code |
| `supermarket_sales.csv` | Dataset |
| `requirements.txt` | Python dependencies |
| `Gajanan_Raje_ProjectReport.docx` | Full project report |
| `README.md` | This file |

## Setup and Run
```bash
git clone <your-repo-url>
cd <repo-folder>
pip install -r requirements.txt
jupyter notebook Gajanan_Raje_SupermarketSalesAnalysis.ipynb
```
In Jupyter choose **Kernel > Restart & Run All**. Keep `supermarket_sales.csv` in the same folder as the notebook.
Running the notebook also saves all 7 charts as PNG files in a `chart_images` folder (zipped as `chart_images.zip`; in Google Colab the zip downloads automatically).

## Key Findings
- Total sales: 244,411.08 from 500 transactions (average sale 488.82, average rating 3.99)
- Top branch: C (Mumbai) with 72,469; lowest: A (Jaipur) with 52,357
- Top categories: Beverages, Personal Care and Dairy; top products: Cheese, Coffee and Shampoo
- Members account for about 59% of sales
- Sales depend more on unit price (correlation 0.72) than on quantity (0.57)
- The data is clean: no missing values, no duplicates, Sales matches Quantity x Unit Price in every row
