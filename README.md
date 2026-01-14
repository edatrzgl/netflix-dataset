# Netflix Content Analysis Dashboard | Power BI

A comprehensive data visualization project analyzing Netflix’s content library from the 2010s onward, using  
**Excel for data cleaning → SQL for data transformation → Power BI for interactive dashboards**.

<img width="1184" height="697" alt="Overview_netflix" src="https://github.com/user-attachments/assets/d186aad6-560d-4ec4-b5c4-6de6a1b07305" />

## Project Objective
To gain insights into movies and TV shows available on Netflix, including:
- How much content was added each year?
- What are the most popular genres?
- How is the content distributed by rating?
- Which countries have access to which content?
- Quickly viewing detailed information for a selected title (cast, director, genres, etc.)

## Technologies & Tools Used
- **Excel** → Data cleaning, trimming whitespace, handling missing values, data restructuring (pivot/unpivot), VLOOKUP, and Pivot Table analysis  
- **SQL** → Data normalization, splitting multi-value fields (cast, director, genres), generating unique keys  
- **Power BI** → Data modeling, DAX measures, interactive slicers, map visualizations, and trend analysis  

## Data Preparation Process (Most Critical Part!)
1. Imported the raw Netflix dataset into Excel  
2. Cleaned whitespace (TRIM) and handled missing/null values  
3. Split multi-value columns such as *Cast*, *Director*, and *Listed In*  
   - Created separate rows for each actor, director, and genre  
   - Assigned unique IDs to make the data suitable for a relational model  
4. Organized cleaned tables into separate sheets (Movies, Cast, Directors, Countries, etc.)  
5. Imported the data into Power BI and built the data model using a **star schema** approach  

## Dashboard Features & Visuals

### 1. Single Title Detail Card (Drill-down)
For a selected movie or TV show:
- Release year and rating (TV-MA, TV-14, etc.)
- Short description  
- Genres  
- Director & cast  
- Availability by country (map visualization)

<img width="1169" height="693" alt="Single_title_netflix" src="https://github.com/user-attachments/assets/21443148-d742-4b54-a9e5-f4dbb374f929" />

### 2. Overall Trends & Statistics
- Number of titles added over time (major growth between 2014–2021)  
- Rating distribution (TV-MA and TV-14 dominate)  
- Top 10 most popular genres (International Movies and Dramas lead)  
- Global content availability map  
