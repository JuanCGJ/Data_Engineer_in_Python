# 🛠️ Data Engineer in Python

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?style=flat&logo=pandas&logoColor=white)
![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-D71F00?style=flat&logo=sqlalchemy&logoColor=white)
![DataCamp](https://img.shields.io/badge/Platform-DataCamp-03EF62?style=flat&logo=datacamp&logoColor=black)
![Courses](https://img.shields.io/badge/Courses-4%20completed-blue?style=flat)
![Level](https://img.shields.io/badge/Level-Beginner%20→%20Intermediate-orange?style=flat)

> **Platform:** DataCamp — *Data Engineer in Python* career track

## 📖 About

This repository documents my progress through DataCamp's **Data Engineer in Python** career track: from cloud fundamentals and core Python to importing data from many sources, on the way to ETL pipelines, Airflow and PySpark.

Each folder contains a **showcase notebook**, not a copy of my notes: a short presentation of what I learned, with runnable code that proves each concept and a closing note on how it applies to a Data Analyst / Data Engineer role.

## 🗂️ Structure

| # | Folder | Course | Showcase notebook |
|---|---|---|---|
| 1 | [1_Understanding_Cloud_Computing](1_Understanding_Cloud_Computing/) | Understanding Cloud Computing | [Cloud_Computing_Showcase.ipynb](1_Understanding_Cloud_Computing/Cloud_Computing_Showcase.ipynb) |
| 2 | [2_Introduction_to_Python_for_Developers](2_Introduction_to_Python_for_Developers/) | Introduction to Python for Developers | [Python_for_Developers_Showcase.ipynb](2_Introduction_to_Python_for_Developers/Python_for_Developers_Showcase.ipynb) |
| 3 | [3_Intermediate_Python_for_Developers](3_Intermediate_Python_for_Developers/) | Intermediate Python for Developers | [Intermediate_Python_Showcase.ipynb](3_Intermediate_Python_for_Developers/Intermediate_Python_Showcase.ipynb) |
| 4 | [4_Introduction_to_Importing_Data_in_Python](4_Introduction_to_Importing_Data_in_Python/) | Introduction to Importing Data in Python | [Importing_Data_Showcase.ipynb](4_Introduction_to_Importing_Data_in_Python/Importing_Data_Showcase.ipynb) |

*More courses will be added as I progress through the track.*

## 📚 Details

### 1. [Understanding Cloud Computing](1_Understanding_Cloud_Computing/Cloud_Computing_Showcase.ipynb)
Conceptual course: cloud value (virtualization, scalability, pay-as-you-go), service models (IaaS, PaaS, SaaS, FaaS), deployment models (public, private, hybrid, multicloud, community), GDPR and personal data, cloud roles, and the Big Three providers (AWS, Azure, Google Cloud) with case studies. The notebook turns the theory into small pandas models: a scaling cost comparison, a responsibility matrix and a provider-service lookup.

### 2. [Introduction to Python for Developers](2_Introduction_to_Python_for_Developers/Python_for_Developers_Showcase.ipynb)
Python fundamentals through a **recipe scaler** project: variables and data types, operators, strings, lists, dictionaries, sets, tuples, conditionals, `for`/`while` loops and workflow keywords (`in`, `not`, `and`, `or`, `.append()`).

### 3. [Intermediate Python for Developers](3_Intermediate_Python_for_Developers/Intermediate_Python_Showcase.ipynb)
Writing reusable, robust code: built-in functions, the `os` and `string` modules, packages and pandas, custom functions (default/keyword arguments, docstrings, `*args`, `**kwargs`), lambda functions with `map()`, and error handling with `try-except` and `raise`.

### 4. [Introduction to Importing Data in Python](4_Introduction_to_Importing_Data_in_Python/Importing_Data_Showcase.ipynb)
Getting data into Python from three kinds of sources: flat files (plain text, NumPy `loadtxt`/`genfromtxt`, pandas `read_csv`), other formats (pickle, Excel, SAS, Stata, HDF5, MATLAB) and relational databases (SQLAlchemy engine, `SELECT`/`WHERE`/`ORDER BY`/`JOIN`, `pd.read_sql_query`). Runs on the 9 course datasets in [`Resources/`](4_Introduction_to_Importing_Data_in_Python/Resources/), including the Chinook SQLite database and LIGO HDF5 data; SQL code uses the current SQLAlchemy 2.x API.

## 🧰 Skills Demonstrated

- Cloud concepts: service and deployment models, scalability, data regulations (GDPR), provider services
- Core Python: data types, data structures, control flow and iteration
- Reusable code: custom functions, docstrings, `*args`/`**kwargs`, lambdas, `map()`
- Defensive programming: `try-except`, `raise`, input validation
- Working with modules and packages (`os`, `string`, pandas, NumPy, SciPy, h5py)
- Data ingestion from CSV/TXT, Excel, SAS, Stata, HDF5, MATLAB and pickle files
- SQL querying from Python with SQLAlchemy and pandas, including joins
- Resource management with context managers (files and database connections)

## 📁 Repository Contents

| Content | Description |
|---|---|
| `*_Showcase.ipynb` | Showcase notebook for each course |
| `chapterN.pdf` | Course theory slides by chapter |
| `glossary.pdf` | Course glossary |
| `*.md` | Personal course notes (Course 1) |
| `Resources/` | Datasets used in the course (Course 4) |

## 🚀 How to Run

```bash
git clone https://github.com/JuanCGJ/Data_Engineer_in_Python.git
cd Data_Engineer_in_Python
pip install -r requirements.txt
jupyter notebook
```

Run each notebook from its own folder so relative paths (e.g. `Resources/`) resolve correctly.

---

*Built with 🤍 as part of a continuous learning journey in Data Engineering.*
