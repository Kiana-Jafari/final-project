# Chicago Data Analysis with SQL (Final Project of: IBM: SQL for Data Science)

This project explores and analyzes multiple public datasets related to Chicago, including census data, crime reports, and public school performance. The analysis is performed using **SQL queries on SQLite**, with the goal of uncovering insights and relationships between demographics, crime, and education in the city.

## Project Structure
- `project.ipynb` → Jupyter Notebook containing SQL queries, explanations, and results  
- Datasets:  
  - `cesus_data.csv` → Census demographics of Chicago  
  - `chicago_crimes_data.csv` → Reported crime records  
  - `chicago_public_schools.csv` → School performance and metrics  

## Features
- SQL-based exploration of Chicago datasets  
- Queries cover joins, aggregations, filtering, and advanced data insights  
- Ready-to-use database import commands for both Python and **raw SQLite terminal** users  

## Usage

### Option 1: Run in Jupyter Notebook
Open `project.ipynb` and execute the cells step by step to replicate the analysis.

### Option 2: Use SQLite directly (no Python required)
You can import the datasets into SQLite tables manually using the commands below:

```
sqlite3 FinalDB.db
.import --csv cesus_data.csv cesus_data
.import --csv chicago_crimes_data.csv chicago_crimes_data
.import --csv chicago_public_schools.csv chicago_public_schools
.tables
```

This will create the following tables in your database:
- cesus_data
- chicago_crimes_data
- chicago_public_schools

From here, you can execute raw SQL queries in the SQLite shell.
