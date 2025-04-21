# Netflix Data Cleaning Project(Using EXCEL)

## Project Description
Cleaned Netflix Movies and TV Shows dataset from Kaggle using Excel.

## Steps Performed
1. Handled missing values
2. Fixed misaligned columns
3. Split duration into value + unit

## Files Included
- `data/raw/netflix_titles.csv`: Original data
- `data/processed/netflix_clean.xlsx`: Cleaned data
- `docs/cleaning_steps.md`: Detailed steps

## Tasks Performed
1.Download the dataset from Kaggle.

2.Imported the dataset to Excel.

3.Checked the dataset for any dublicate datas.
  By using the data tools in data option.
  
4.Checked the columns for extra spaces and Standerdizing the names/title of the movies ot tv-series.
  For Removing extra spaces Formula(=TRIM(INDEX PLACE)).
  For standersizing the text Formula(=PROPER(INDEX PLACE)).
  
5.Removed all Blank values will "Unknown" in the Datasets.

6. Converted the Added-Date into DateTime format.
7. 
   Formula(=TEXT(DATE(RIGHT(h1,4), MONTH(1 & MID(h1,1,FIND(" ",h1)-1)), MID(h1,FIND(" ",h1)+1,FIND(",",h1)-FIND(" ",h1)-1)), "dd/mm/yyyy").
   
9. Removed all the data tangaled between Rating and Duration column .By using Find and Replace method .
  
11. Converted the Duration column into two groups Duration_value and Duration_Units. 


