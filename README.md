# Jupyter_Notebook_Project
This project showcases my proficiency to perform EDA and data visualization on Python.

## Analysis on Forbes Top 2000's Companies
[[Analysis on Forbes Top 2000 Companies.ipynb]](https://github.com/zhi-hern/JupyNotebook_Project/blob/main/Analysis%20on%20Forbes%20Top%202000%20Companies.ipynb) <br>
[[Data from Kaggle]](https://www.kaggle.com/datasets/mohammadgharaei77/largest-2000-global-companies/data) <br>
[[Reference]](https://www.forbes.com/lists/global2000/)

### Data Dictionary:
| Column name | Description |
| -------- | ----------- |
| Rank    | Forbes' ranking based on 4 metrics: <br> (i) Sales (ii) Profit (iii) Assets (iv) Market Value|
| Name    | Company's Name |
| Sales  | Sales (in Billions) of Dollars  |
| Profit | Profit (in Billions) of Dollars | 
| Assets | Assets (in Billions) of Dollars |
| Market Value | Market Value (in Billions) of Dollars |
| Industry | Company's Industry |
| Founded | Year Established |
| Headquarters | Location of Company's Headquarters |
| Country | Country of Company's Headquarters |
| CEO | Company's current CEO |
| Employees | Current number of employees |

### Steps Performed:
- `Pandas` was used to create a dataframe.

- Exploring the data: 
`.info()` method was used to identify the data types and size of the datasets.

- `Drop()` method was used to delete unnecessary columns for this analysis. (i.e: 'CEO', 'Employees')
  
- `Rename()` method was used to rename 'Sales', 'Profit', 'Assets' & 'Market Values' columns.
  
- `Duplicated()` method was use to determine any duplicated values.

- Exploring the industries of top 2000 companies using `set`.

- Aggregate similar industries into one for further analysis.

- Validate data by searching the web.

