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

### Libraries Used
| Library        | Method Used         |
| --------       | ------------------- |
| Pandas (pd)    | `.read_csv()`, `.info()`, `.drop()`, `.head()`, `.rename()`<br> `.duplicated()`, `.replace()`, `.isnull()`, `.loc[]`<br> `.value_counts()`, `reset_index()`, `.groupby()`, `.sort_values()`, <br> `.astype()`, `.describe()`, `.insert()`, `.agg()`, `.merge()` |
| Matplotlib.pyplot (plt)| `.figure()`, `.xlabel()`, `.ylabel()`, `.title()` , `.xticks()` |
| Seaborn (sns)  | `.barplot()`, `.boxplot()` |

### Further financial analysis:
- Perplexity AI was used to suggest some financial method to further analyze the companies.
- Below shows the index used in this project with some assumptions made :

<img width="512" alt="image" src="https://github.com/user-attachments/assets/18b1384b-359f-4bad-a1df-4bb9b55db5c9"> <br>
<img width="484" alt="image" src="https://github.com/user-attachments/assets/a9757dab-cd68-4bb6-8b51-33e9fad0b161"> <br>
<img width="496" alt="image" src="https://github.com/user-attachments/assets/61741fff-9987-40b6-9238-bb8635cbd745">

