# Netflix Data Analysis Project

## 📖 Overview

This project provides insights into Netflix's content library using SQL queries executed on a PostgreSQL database. The analysis explores various aspects of the Netflix dataset, including content type distribution, popular ratings, top countries by content volume, and more. The project uses **PostgreSQL** for database management and **pgAdmin 4** as the graphical user interface for database operations.

---

## 💾 Software and Tools Used

- **PostgreSQL**: Open-source relational database management system.
- **pgAdmin 4**: Web-based GUI for managing PostgreSQL databases.
- **SQL**: Structured Query Language for querying and managing the database.


---

## 🚀 How to Run the Project

1. **Install PostgreSQL and pgAdmin 4**

   - Download and install [PostgreSQL](https://www.postgresql.org/download/) according to your operating system.

2. **Set Up the Database**

   - Open pgAdmin 4 and create a new database (`netflix_db`).
   - Import the `netflix data.xlsx` dataset into the database (you can use the import/export tool in pgAdmin 4).

3. **Run the SQL Queries**

   - Open `analysis_queries.sql` in pgAdmin 4's query tool.
   - Execute the queries to generate the analysis results.

4. **View the Results**

   - Results will be stored in the `Netflix Data Analysis` pdf file.

---

## 🚀 Features

- 📊 **Content Distribution**: Analyze the number of movies vs. TV shows.
- ⭐ **Ratings Analysis**: Identify the most common ratings for both movies and TV shows.
- 🎬 **Year-wise Content Listing**: Filter movies by specific release years.
- 🌏 **Top Countries**: Determine the top 5 countries with the most Netflix content.
- 🕒 **Longest Movie Identification**: Find the longest movie on the platform.
- 🎥 **Director-Specific Content**: List all content by specific directors.
- 📺 **TV Show Analysis**: Find TV shows with more than 5 seasons.
- 🎭 **Genre Distribution**: Count content items by genre.
- 🇮🇳 **India-specific Trends**: Analyze average content release in India by year.
- 🎞 **Documentary Listings**: Retrieve all documentaries available.
- ❓ **Missing Data Analysis**: Identify content without director information.
- 🌟 **Actor Analysis**: Track appearances of popular actors like Salman Khan in the last decade.
- 🎭 **Top Actors in India**: Identify the top 10 actors in Indian-produced content.
- ⚠️ **Content Categorization**: Classify content based on keywords like 'kill' and 'violence.'

---

## 📈 Sample SQL Queries

```sql
-- Count the number of Movies vs TV Shows
SELECT
    type,
    COUNT(*)
FROM netflix
GROUP BY 1;
---

## 📝 License

Distributed under the MIT License.
