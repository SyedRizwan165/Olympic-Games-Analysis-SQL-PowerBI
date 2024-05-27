# Olympic Games Analysis Dashboard-MySQL-PowerBI

Imagine working as a data analyst at a xyz company, the task is to create visualizations that help readers understand the historical performance of countries in the Summer Olympic Games. The primary objective is to showcase the historical performance of various countries, allowing readers to select and focus on specific countries of their choice.

The dataset is taken from https://www.dropbox.com/s/3sxwx52o3x8ozj7/olympic_games.bak?e=1&dl=0

# Data Cleaning

- The data collected was first entered in to the SQL database, where it was cleaned and transformed using the transformation shown below

# Measures Using DAX

The following measures were created using DAX ( Data Analysis Expressions).

### Number Of Participants
- No. Of Players = DISTINCTCOUNT('Olympic Games'[ID])

### Number of Medals
- No. of Medals = COUNTROWS('Olympic Games') 
- No. of Medals won = CALCULATE([No. of Medals] , FILTER('Olympic Games' , 'Olympic Games'[Medal] = "Bronze" || 'Olympic Games'[Medal] = "Silver" || 'Olympic Games'[Medal] = "Gold"))

# Dashboard

The finished dashboard consist of visualization and filters that helps to navigate the summer games through history. You can filter by year, nation code for looking out for a specific country , specific participant or sports.

![image](E:\Olympic games analysis\1.png)# Olympic-Games-Analysis-SQL-PowerBI
