# Project Data Engineering in Python (IBM course) 

## Scenario

An international firm that is looking to expand its business in different countries across the world has recruited you. You have been hired as a junior Data Engineer and are tasked with creating an automated script that can extract the list of all countries in order of their GDPs in billion USDs (rounded to 2 decimal places), as logged by the International Monetary Fund (IMF). Since IMF releases this evaluation twice a year, this code will be used by the organization to extract the information as it is updated.

You can find the required data on this webpage : https://web.archive.org/web/20230902185326/https://en.wikipedia.org/wiki/List_of_countries_by_GDP_%28nominal%29.

The required information needs to be made accessible as a JSON file 'Countries_by_GDP.json' as well as a table 'Countries_by_GDP' in a database file 'World_Economies.db' with attributes 'Country' and 'GDP_USD_billion.'

Your boss wants you to demonstrate the success of this code by running a query on the database table to display only the entries with more than a 100 billion USD economy. Also, log the entire process of execution in a file named 'etl_project_log.txt'.

You must create a Python code 'etl_project_gdp.py' that performs all the required tasks.

* Original Author : Abhishek Gagneja


## Set the Environment and Install Dependencies

```bash
python -m venv virtual-env
source virtual-env/activate
pip install -r requirements.txt
```

## Launch the Script

```bash
python etl_project_gpd.py
```

### Deliverable

The ETL process will produce a final csv file with the following format :

```
,Country,GDP_USD_billions
0,United States,26854.6
1,China,19373.59
2,Japan,4409.74
3,Germany,4308.85
4,India,3736.88
5,United Kingdom,3158.94
6,France,2923.49
7,Italy,2169.74
[...]
```