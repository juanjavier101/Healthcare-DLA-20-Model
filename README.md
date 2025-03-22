# DLA-20 Healthcare Data Model

This repository contains the schema and sample data for a relational database designed to store and manage healthcare information, specifically focusing on patient demographics, DLA-20 mental health assessments, medication history, and hospital readmissions.

## Overview

The purpose of this data model is to provide a structured and efficient way to store and query healthcare data for analysis and reporting. It is designed to be flexible and scalable, allowing for the addition of new data elements and tables as needed.

## Repository Structure


dla20-healthcare-model/
├── sql/
│   ├── schema/
│   │   ├── 01_patients.sql         # Patient table
│   │   ├── 02_assessments.sql      # DLA-20 assessments
│   │   ├── 03_medications.sql      # Medication data
│   │   ├── 04_readmissions.sql     # Hospital readmissions
│   │   └── constraints.sql         # Foreign keys & indexes
│   ├── sample_data/
│   │   └── inserts.sql             # Sample patient, assessment, medication, and readmission data
│   ├── queries/
│   │   └── analytical_queries.sql # More complex queries
│   └── data_validation/
│       └── validation_checks.sql # SQL to check data integrity
├── docs/
│   ├── ER_Diagram.png              # Data model visualization
│   └── data_dictionary.md          # Field descriptions
├── .gitignore
├── LICENSE
└── README.md                       # Project overview & setup guide

## Getting Started

1.  **Clone the repository:**

    ```bash
    git clone [https://github.com/yourusername/dla20-healthcare-model.git](https://github.com/yourusername/dla20-healthcare-model.git)
    ```

2.  **Set up your database:**

    * Ensure you have a relational database system (e.g., MySQL, PostgreSQL, SQLite) installed and configured.
    * Create a new database for the DLA-20 healthcare model.

3.  **Run SQL scripts:**

    * Navigate to the `sql/schema/` directory.
    * Execute the SQL scripts in the following order:

        ```sql
        01_patients.sql
        02_assessments.sql
        03_medications.sql
        04_readmissions.sql
        constraints.sql
        ```

    * Navigate to the `sql/sample_data/` directory.
    * Run the `inserts.sql` script to populate the database with sample data.

4.  **Explore the data:**

    * Use the example queries in `sql/queries/analytical_queries.sql` to explore the data and gain insights.

## Key Tables

* **Patients:** Stores patient demographics and admission/discharge information.
* **Assessments:** Contains DLA-20 mental health assessment scores and clinician notes.
* **DLA20_Responses:** Stores individual responses to DLA20 questions.
* **Medications:** Tracks medication prescriptions and administration.
* **Readmissions:** Records hospital readmission events.

## Documentation

* **ER Diagram:** The `docs/ER_Diagram.png` file provides a visual representation of the database schema and relationships between tables.
* **Data Dictionary:** The `docs/data_dictionary.md` file contains detailed descriptions of each field in the tables.

