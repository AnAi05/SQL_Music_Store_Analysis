# Music Store Database

This repository contains the SQL script to set up a Music Store database. The database includes tables for storing information about albums, artists, and customers. This setup is useful for managing a music store's inventory, customer information, and sales data.

## Database Schema

The database consists of the following tables:

1. **album**
    - `album_id`: VARCHAR(50), Primary Key
    - `title`: VARCHAR(120)
    - `artist_id`: VARCHAR(30), Foreign Key references `artist(artist_id)`

2. **artist**
    - `artist_id`: VARCHAR(50), Primary Key
    - `name`: VARCHAR(120)

3. **customer**
    - `customer_id`: INTEGER, Primary Key
    - `first_name`: CHAR(50)
    - `last_name`: CHAR(50)
    - `company`: VARCHAR(120)
    - `address`: VARCHAR(120)
    - `city`: VARCHAR(50)
    - `state`: VARCHAR(50)
    - `country`: VARCHAR(50)
    - `postal_code`: VARCHAR(50)
    - `phone`: VARCHAR(50)
    - `fax`: VARCHAR(50)
    - `email`: VARCHAR(50)
    - `support_rep_id`: INTEGER

## Prerequisites

To use this script, you need to have a PostgreSQL database installed on your system. You can download and install PostgreSQL from [here](https://www.postgresql.org/download/).

## Setup Instructions

1. **Clone the repository**
    ```bash
    git clone https://github.com/yourusername/music_store_database.git
    cd music_store_database
    ```

2. **Create the database**
    Open the PostgreSQL command line interface (psql) and create the `music_database`.
    ```sql
    CREATE DATABASE music_database;
    ```

3. **Run the SQL script**
    Execute the SQL script to create the tables and insert data (if any).
    ```bash
    psql -d music_database -f Music_Store_database.sql
    ```

## Usage

After setting up the database, you can interact with it using SQL queries. Here are some example queries:

- **Select all albums**
    ```sql
    SELECT * FROM album;
    ```

- **Select all artists**
    ```sql
    SELECT * FROM artist;
    ```

- **Select all customers**
    ```sql
    SELECT * FROM customer;
    ```

## Contributing

If you want to contribute to this project, please fork the repository and create a pull request with your changes. Make sure to follow the coding standards and write meaningful commit messages.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.



Schema- Music Store Database  
![MusicDatabaseSchema](https://user-images.githubusercontent.com/112153548/213707717-bfc9f479-52d9-407b-99e1-e94db7ae10a3.png)
