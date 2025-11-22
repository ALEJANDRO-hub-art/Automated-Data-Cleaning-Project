📊 **Automated Data Cleaning Project**


📘 **Project Overview**

This project focuses on automating data cleaning and standardization within a MySQL environment using:

- Stored Procedures
- Events (scheduled automation)
- Triggers (automatic execution on data change)

The goal is to take a raw dataset (us_household_income) and automatically:

- copy it into a cleaned version
- remove duplicate records
- standardize inconsistent text values
- maintain ongoing data quality without manual effort
- allow future inserts to be processed automatically

The script builds a fully automated pipeline where MySQL handles data cleaning internally, reducing the need for external tools or repeated manual SQL execution. 


🧩 **Business Problem**

Real-world datasets—especially large demographic or government data like U.S. Household Income—commonly suffer from:

- duplicated rows
- inconsistent text formatting
- misspellings
- structural issues
- manual reporting delays
- repeated cleaning effort

**Without automation:**

- analysts repeatedly clean the same data
- reports become inconsistent
- errors propagate into dashboards and models
- manual labor increases cost and time

The business need is:
- a reliable, repeatable, automated process that ensures the dataset is always clean and standardized before use in analytics, reporting, machine learning, or integration pipelines.

⚙️ Tech Stack

MySQL Database

**Used for:**
- data storage
- transformation
- automation logic

**Stored Procedures**

- Automate multi-step cleaning operations:
- create cleaned table
- copy data
- remove duplicates
- standardize values

**Events (MySQL Scheduler)**

Automated recurring execution:
