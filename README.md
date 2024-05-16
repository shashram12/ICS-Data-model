# ICS-Data-model

## Overview
- Information Competition Simulator (ICS) is a software that is designed for modeling human behaviour. It simulates how information propagates through a network and affects how the opinions of target population (collection of “agents”) change in relation to the topics in shared messages.
- Consists of thousands of agents who are initialised with a certain of set parameters (opinions and beliefs). 
- The process of selecting and initialising the parameters for any scenario needed improvements. Currently, there is a lack of automation in absorbing data from source files, which often exist in different formats. Our project is centered around enhancing this process.

## Specifics about data

We have focused particularly on the region of Morocco, for which we were able to obtain data from multiple barometers' websites:

- [WVS Wave 7](https://www.worldvaluessurvey.org/WVSDocumentationWV7.jsp)
- [Afrobarometer](https://www.afrobarometer.org/survey-resource/morocco-round-9-data-2023/)
- [Arabbarometer wave 7](https://www.arabbarometer.org/survey-data/data-downloads/)

After running the python scripts the following five tables are populated with data and metadata from the source files:

- Dimension_value_morocco
- survey_questions_morocco
- response_values_morocco
- scenario_qids
- Scenarios

## Running the code files

- Run the Code Files
- Install PostgreSQL.
- Create Database.
- Download all source files and add them to your Colab notebook/Python Environment.
- Run pip install pandas, pyreadstat, sqlalchemy to install necessary libraries.
- In the connection string, ensure you have the right database connection.
- Run the code, and the relevant tables should be populated in your database.
