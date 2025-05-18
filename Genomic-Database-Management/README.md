# Integrating MySQL and REST APIs for Biological Data Analysis

## Description
This project demonstrates the integration of MySQL database management and REST APIs to analyze biological data. By combining data from local CSV files and public REST services, it constructs relational databases and processes information on genes, proteins, and amino acid sequences.

## Objectives

- Create and manage MySQL relational tables for biological datasets.
- Populate databases with information from CSV files and REST API services.
- Develop an interactive Python script for exploring gene-protein relationships and protein sequences.
- Evaluate REST API responses for consistency and reliability.

## Techniques and Libraries

- **Database Management:** MySQL, MySQL Connector.
- **Data Integration:** CSV parsing, REST API consumption.
- **Programming Tools:** Python, requests, csv, mysql.connector, Jupyter Notebook.

## Repository Structure

- `Scripts/`: Contains Jupyter Notebook files `Parte1.ipynb` and `Parte2.ipynb` used for database management and querying.
- `Data/`: Contains the input file `genes.csv` for populating the gene table.

## How to Reproduceç

1. **Clone the repository:**
   ```bash
   git clone https://github.com/anam16/biological-data-analysis.git
   cd biological-data-analysis/
   
2. Set up MySQL database:
Install MySQL and create a database with a user account.

3. Install dependencies:
   ```bash
   pip install mysql-connector-python requests notebook
   
4. Run the analysis in Jupyter Notebook:
   Launch Jupyter Notebook by running:
   ```bash
   jupyter notebook
   
Navigate to the Scripts/ folder and open `Parte1.ipynb` and `Parte2.ipynb`.
Execute the notebook cells sequentially to perform database setup, data ingestion, REST API queries, and data analysis.
