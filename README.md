# Music Recommendation ETL Pipeline

![Python](https://img.shields.io/badge/python-3.12-blue)
![ETL](https://img.shields.io/badge/ETL-pipeline-green)
![DIO Bootcamp](https://img.shields.io/badge/DIO-Santander%20Bootcamp-orange)

Project created for the Data Science DIO Santander Bootcamp 2025 ETL challenge.

Simple ETL pipeline to generate personalized music recommendations using **Groq AI**.

## Overview

- **Extract:** Load user data from `music_sentiment.csv`
- **Transform:** Clean and standardize `fav_genre` and `mood`, create AI prompts
- **Load:** Generate recommendations using Groq AI and save to `music_recommendations.csv`

## Example Input

| user_id | user  | fav_genre  | mood   |
|---------|-------|------------|-------|
| 1       | Ana   | Pop        | Happy |
| 2       | João  | Rock       | Tired |

## Example Output

| user_id | user  | fav_genre  | mood   | recommendations |
|---------|-------|------------|-------|----------------|
| 1       | Ana   | Pop        | Happy | “Can’t Stop the Feeling!” – Justin Timberlake ... |
| 2       | João  | Rock       | Tired | **Eye of the Tiger** – Powerful anthem ...        |

## Usage

1. Add your **Groq API key** in the script.
2. Run the notebook to generate recommendations.
3. Output saved in `music_recommendations.csv`.
