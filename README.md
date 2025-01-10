# Jupyter_Notebook_Project
This project showcases my proficiency to perform EDA and data visualization using Python.

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

### Libraries Used
| Library        | Method Used         |
| --------       | ------------------- |
| Pandas (pd)    | `.read_csv()`, `.info()`, `.drop()`, `.head()`, `.rename()`<br> `.duplicated()`, `.replace()`, `.isnull()`, `.loc[]`<br> `.value_counts()`, `reset_index()`, `.groupby()`, `.sort_values()`, <br> `.astype()`, `.describe()`, `.insert()`, `.agg()`, `.merge()` |
| Matplotlib.pyplot (plt)| `.figure()`, `.xlabel()`, `.ylabel()`, `.title()` , `.xticks()` |
| Seaborn (sns)  | `.barplot()`, `.boxplot()` |

### Steps taken for the EDA process

The EDA process I took roughly follows the steps outlined below:

<img width="727" alt="EDA-6-stages" src="https://github.com/user-attachments/assets/127af722-7113-4248-b4ef-d7c7ef743e4a" />

#### 1) Discovering :
- After the data was imported into a dataframe, data was explored using `.info()`.
  Through exploring the dataset, I know the shape, size, type of data in the dataset. I can determine the the null values too.

  <img width="337" alt="image" src="https://github.com/user-attachments/assets/5f339a7e-fb89-489f-88ec-33af30ee98af" />

From this, 2001 rows and 12 columns in the dataset were determined. Several null values in the 'Industry', 'Founded', 'Headquarters', 'CEO' and 'Employees' columns were discovered too.

- Checked for duplicates using `.duplicated()` method and no duplicate was found.

#### 2) Structuring:
- Restructred the dataset by dropping the columns that are not involved in my analysis using `.drop()`.

#### 3) Cleaning: 
- 'Sales', 'Profit', 'Assets', and 'Market Values' columns were renamed by adding '(In Billions)' at the end to improve clarity of the data.
- Structured the dataset by aggregating simliar industry for further analysis.
(Eg. Grouping "Auto Brands", "Auto Parts", "Automotive (Automotive and Suppliers)", "National Car Dealers" into 1 category: "Automotive".)
- Boxplot was plotted for 'Founded' column and found out there is a outlier in the dataset. `.describe()` method was used to identify the exact value of the outlier.
  Obviously, this is a typo in the dataset. By searching the company info via internet, the founded year of the company was identified and corrected.  
  
  <img width="467" alt="image" src="https://github.com/user-attachments/assets/7ddbffd5-18b6-4498-9f42-dbb4f96376d1" /> <br>
  <img width="396" alt="image" src="https://github.com/user-attachments/assets/a3417417-7d58-4e19-95fa-9c35ae979317" /> <br>
  <img width="755" alt="image" src="https://github.com/user-attachments/assets/8d59f031-ae0c-453f-b5b8-03c162ae7d94" /> <br>
  <img width="682" alt="image" src="https://github.com/user-attachments/assets/de23ea03-cdfc-4928-8af7-4347edfe32c6" />

#### 4) Validating:
-  Rows that contain null values were filtered using `.isnull()`.
-  Null values in the 'Industry' and 'Founded' columns were filled by Googling the companies' info.

#### 5) Exploring for Presentation:
 
#### 6) Visualize data for Presentation:

### Findings
- Finance companies, i.e.: Banking (354 Banking companies made it in the Top 2000 list) and Diversified Financials (117 Diversified Financials companies made it in the Top 2000 list) dominate the top 2000 companies' list.
  
    <img width="316" alt="image" src="https://github.com/user-attachments/assets/04e86310-05e8-4f7e-8837-1d055cefa29f" />

- Top 5 most profitable industries are: Conglomerate, Specialty, Construction- Chemicals- Raw Materials, Semiconductors & Automotive.

    <img width="383" alt="image" src="https://github.com/user-attachments/assets/35268359-0616-4de8-8e9e-e3ac8ed35848" />


### Further financial analysis:
- Perplexity AI was used to suggest some financial method to further analyze the companies.
- Below shows the index used in this project with some assumptions made :

<img width="512" alt="image" src="https://github.com/user-attachments/assets/18b1384b-359f-4bad-a1df-4bb9b55db5c9"> <br>
<img width="484" alt="image" src="https://github.com/user-attachments/assets/a9757dab-cd68-4bb6-8b51-33e9fad0b161"> <br>
<img width="496" alt="image" src="https://github.com/user-attachments/assets/61741fff-9987-40b6-9238-bb8635cbd745">

