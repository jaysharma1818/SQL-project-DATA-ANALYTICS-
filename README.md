# SQL-project-DATA-ANALYTICS-

# Music Store Database Analysis (MySQL)

This project contains a collection of **MySQL queries** used to analyze a music store database.  
The analysis is performed using data imported from CSV files and focuses on **customers, invoices, artists, genres, and sales insights**.

---

## 📁 Project Structure
├── csv/
│ ├── Album1.csv
│ ├── Artist.csv
│ ├── Customer.csv
│ ├── Employee.csv
│ ├── Genre.csv
│ ├── Invoice.csv
│ ├── Invoice_Line.csv
│ └── Track.csv
│
├── music_store_analysis.sql
└── README.md
---


## 🛠️ Technologies Used
- **MySQL 8.0**
- **SQL (CTEs, Joins, Aggregations, Window Functions)**
- **CSV files for data loading**



📊 Analysis Performed
This project answers real-world business questions such as:

🎵 Top-selling artist by total revenue
👤 Best customer based on total spending
🌍 Top customer in each country
🎼 Most popular genre by country
🎸 Artists with the most Rock songs
🧾 Top invoices and city-wise revenue
⏱️ Tracks longer than average duration



## 🗄️ Database Setup
1. Create the database:
```sql
CREATE DATABASE jaydb;
USE jaydb;

CREATE TABLE album1 (
  album_id INT PRIMARY KEY,
  title VARCHAR(255),
  artist_id INT
);

LOAD DATA INFILE 'path_to_csv/Album1.csv'
INTO TABLE album1
FIELDS TERMINATED BY ','
ENCLOSED BY '"'
LINES TERMINATED BY '\n'
IGNORE 1 ROWS;






