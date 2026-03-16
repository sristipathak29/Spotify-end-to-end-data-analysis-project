# Spotify Music Streaming Analysis (SQL Project)

## Project Overview
This project explores a dataset inspired by Spotify music streaming data to analyze song performance, artist popularity, and music characteristics using SQL.

The goal of this project is to practice real-world data analysis using SQL by answering business-style questions such as:
- Which songs have the highest streams?
- Which artists dominate the platform?
- How do music features like energy and danceability relate to popularity?

The analysis was performed entirely using SQL queries.

---

## Dataset
The dataset contains 10,000 simulated Spotify track records with the following attributes:

| Column | Description |
|------|-------------|
| track_id | Unique identifier for each track |
| track_name | Name of the song |
| artist_name | Artist performing the track |
| release_year | Year the track was released |
| popularity | Popularity score (0-100) |
| danceability | Danceability score |
| energy | Energy level of the track |
| tempo | Beats per minute |
| duration_ms | Track duration in milliseconds |
| streams | Total number of streams |

Each record represents a song available on Spotify.

---

## Tools Used
- SQL
- MySQL
- Data Analysis

---

## Key Business Questions Answered

### Data Exploration
- Total number of songs in the dataset
- Number of songs released each year
- Average popularity of songs
- Average tempo and duration of songs

### Artist Analysis
- Top artists with the most songs
- Top artists by total streams
- Artists with the highest average popularity

### Song Performance
- Top 10 most streamed songs
- Songs with popularity greater than 90
- Songs longer than 4 minutes

### Music Feature Analysis
- Songs with high energy
- Songs with high danceability
- Songs where energy is greater than danceability

### Advanced SQL Analysis
--Songs with Tempo above average'
-- Songs Longer Than Average Duration

## Example SQL Query

Top 10 most streamed songs:

```sql
SELECT track_name, artist_name, streams
FROM spotify_records
ORDER BY streams DESC
LIMIT 10;
