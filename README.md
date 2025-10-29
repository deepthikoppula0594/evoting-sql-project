# E-Voting System Data Analysis (Using MySQL)

## Overview
This project analyzes real-world U.S. election data using MySQL.  
The dataset, sourced from Kaggle, contains state-wise election results including candidate names, parties, and vote counts.  
The goal is to perform SQL-based analysis such as vote counting, party performance, and state-level insights.

---

## Dataset
- **Source:** [US Elections Dataset on Kaggle](https://www.kaggle.com/datasets/tunguz/us-elections-dataset)
- **Direct Download Link:** [Download Dataset (ZIP)](https://www.kaggle.com/datasets/tunguz/us-elections-dataset/download?datasetVersionNumber=1)
- **Columns Used:**
  1) year  
  2) state  
  3) office  
  4) candidate  
  5) party_simplified  
  6) candidatevotes  
  7) totalvotes  

---

## SQL Schema
```sql
CREATE TABLE Votes (
    vote_id INT AUTO_INCREMENT PRIMARY KEY,
    year INT,
    state VARCHAR(50),
    office VARCHAR(100),
    candidate VARCHAR(100),
    party_simplified VARCHAR(50),
    candidatevotes INT,
    totalvotes INT
);
