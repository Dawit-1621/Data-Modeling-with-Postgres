# Data Modeling with Postgres
#### What is data modeling?
Data modeling is the process of creating a visual representation of either a whole information system or parts of it to communicate connections between data points and structures. The goal is to illustrate the types of data used and stored within the system, the relationships among these data types, the ways the data can be grouped and organized, and its formats and attributes. <br>

#### What is PostgreSQL?
PostgreSQL is a powerful, open-source object-relational database system with over 35 years of active development that has earned it a strong reputation for reliability, feature robustness, and performance. <br>


#### Overview of the project
An overview of the steps involved in performing data modeling with Postgres, creating a star schema database, and building an ETL (Extract, Transform, Load) pipeline using Python for Sparkify. <br>
1. Define Schema:
* Identify the entities and their relationships within Sparkify's data (e.g., songs, artists, users, time, and songplays).<br>
* Create a logical schema that represents these entities and relationships. For instance:<br>
     * `Songs table`
     * `Artists table`
     * `users table`
     * `timetable`
     * `songplays fact table`
2. Creating a Star Schema Database: <br>
a. Implement Star Schema:<br>
Transform the logical schema into a star schema design where a central fact table (e.g., songplays) is surrounded by dimension tables (e.g., `songs`, `artists`, `users`, `time`).
Connect dimension tables to the fact table using foreign keys.
Ensure denormalization in dimension tables for easier querying and analysis.

#### Dataset
The file name, mini_sparkify_event_data.json, will be loaded and cleaned such as handling invalid or missing values.
