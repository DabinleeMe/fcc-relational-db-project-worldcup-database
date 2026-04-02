# ⚽ World Cup Database

This project is part of the **freeCodeCamp - Relational Database Certification**. It focuses on building a PostgreSQL database from scratch and automating data ingestion from a CSV file using a professional Bash script.

## 🚀 Key Features

* **Database Schema Design**: Designed a relational schema with two linked tables (`teams` and `games`) using **Primary Keys** and **Foreign Keys** to ensure data integrity.
* **Automated Data Ingestion**: Developed `insert_data.sh`, a robust Bash script that parses `games.csv` and populates the database automatically.
* **Relational Logic**: 
    * Implemented logic to check for existing records before insertion to avoid duplicates (**Unique Constraints**).
    * Handled complex many-to-one relationships between teams and games.
* **Advanced SQL Querying**: Created `queries.sh` to extract meaningful insights (e.g., total goals, winning streaks, tournament winners) using **JOINs**, **GROUP BY**, and **Subqueries**.

## 🛠 Tech Stack & Tools

* **PostgreSQL**: For relational database management.
* **Bash (Linux Terminal)**: To automate the ETL (Extract, Transform, Load) process.
* **SQL**: For schema definition and complex data retrieval.
* **Git & GitHub**: For version control and documentation.

## 📁 Project Components

* **`worldcup.sql`**: The complete database schema export.
* **`insert_data.sh`**: The Bash script that reads the CSV and inserts data into SQL.
* **`games.csv`**: The raw data containing World Cup match results from 2014 and 2018.
* **`queries.sh`**: A collection of SQL queries for data analysis.

## 📖 How to Set Up

1.  **Clone the repository**:
    ```bash
    git clone [https://github.com/DabinleeMe/fcc-relational-db-project-worldcup-database.git](https://github.com/DabinleeMe/fcc-relational-db-project-worldcup-database.git)
    ```
2.  **Rebuild the database**:
    ```bash
    psql -U postgres < worldcup.sql
    ```
3.  **Run the insertion script**:
    ```bash
    chmod +x insert_data.sh
    ./insert_data.sh
    ```
4.  **Run queries to see results**:
    ```bash
    ./queries.sh
    ```

---
*Developed by Dabin Lee. This project demonstrates proficiency in SQL database management and automation for business intelligence.*
