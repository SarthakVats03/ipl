# IPL Database Management System

### Overview
This project involves the design and implementation of a **Database Management System (DBMS)** for the **Indian Premier League (IPL)**. The system helps manage information related to matches, players, teams, and statistics. It aims to streamline the process of maintaining tournament records and generating insights for better tournament management.

### Features
- **Comprehensive Player Records**: Track every player's stats, performance, and team affiliation.
- **Match Management**: Store and manage details of matches including teams, venues, and match statistics.
- **Team Standings and Points Table**: Maintain up-to-date points and rankings for all IPL teams.
- **Performance Metrics**: Track key statistics such as runs, wickets, strike rates, and net run rates (NRR).
- **Queries for Data Retrieval**: Predefined queries to fetch specific information from the database (e.g., top players, team standings, or season winners).

---

## Table of Contents
1. [Problem Statement](#problem-statement)  
2. [Assumptions](#assumptions)  
3. [ER Diagram](#er-diagram)  
4. [Relational Schema](#relational-schema)  
5. [Normalization](#normalization)  
6. [Table Structure](#table-structure)  
7. [Insertions and Sample Data](#insertions-and-sample-data)  
8. [Predefined Queries](#predefined-queries)  
9. [How to Run](#how-to-run)  
10. [Future Enhancements](#future-enhancements)

---

## Problem Statement
The goal of this project is to create a database for the **IPL** that allows the **Board of Control for Cricket in India (BCCI)** to efficiently manage player records, match statistics, and tournament standings. It helps in:
- Maintaining individual and team performance data.
- Keeping track of all matches and results.
- Facilitating the generation of points tables and awards.

---

## Assumptions
- A player belongs to only one team during a season (1:M relationship).
- A venue can host multiple matches, but each match occurs at a single venue (M:1 relationship).
- A match involves two teams, and each match’s statistics are stored separately (M:N relationship).
- Points are derived based on wins and losses, and rankings are based on points and NRR.

---

## ER Diagram
Refer to the [ER Diagram](#) (insert the diagram link or image here) for a visual representation of the relationships among entities.

---

## Relational Schema
The project follows **relational schema design** to ensure organized data storage:
- **Teams Table**: Stores team details and codes.
- **Players Table**: Stores player details such as name, nationality, and performance metrics.
- **IPLMatch Table**: Stores match details including participating teams and venues.
- **Statistics Table**: Captures detailed statistics for every match.
- **Points Table**: Tracks points and standings of each team.

---

## Normalization
- **BCNF and 3NF Normalization** applied to relevant tables.
- **Partial and Transitive Dependencies** eliminated to maintain data integrity and reduce redundancy.

---

## Table Structure
- **Teams Table**  
- **Players Table**  
- **Venues Table**  
- **Points Table**  
- **Matches Table**  
- **Statistics Table**  

All tables use **foreign key constraints** to ensure referential integrity.

---

## Insertions and Sample Data
Sample data for players, teams, matches, and statistics is included to demonstrate how the system operates. Please refer to the project documentation for the specific **SQL INSERT statements**.

---

## Predefined Queries
Here are some predefined SQL queries included in the project:
1. **Find Indian players from CSK.**  
2. **Get the top 10 players by total runs.**  
3. **Display MI players sorted by age.**  
4. **Find the youngest and oldest players.**  
5. **Show details of all matches.**  
6. **Retrieve players from RCB or CSK.**  
7. **Query the season winner.**

---

## How to Run
1. Install a **MySQL/MariaDB** server (or any SQL-compatible DBMS).
2. Create the required tables by executing the provided SQL scripts.
3. Insert sample data using the provided SQL statements.
4. Run the predefined queries to verify the database functionality.

---

## Future Enhancements
- **Dynamic Team Management**: Adding features to track player transfers between teams.
- **Live Match Updates**: Integrating APIs for real-time statistics and match updates.
- **Web Interface**: Develop a frontend to interact with the database via a web-based dashboard.
- **Data Analytics**: Introduce predictive analytics for player and team performance.

---

## Authors and Acknowledgments
This project was created to demonstrate the principles of **Database Management Systems** and its applications in sports management. Special thanks to the BCCI for the IPL framework and resources.

---

## License
This project is licensed under the MIT License - see the [LICENSE](#) file for details.
