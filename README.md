# GT World Challenge Europe Data Analysis | Web Scraping Project



## Project Overview
This project is designed to identify the most optimal GT3 car for participation in the [GT World Challenge Europe](https://www.gt-world-challenge-europe.com/results) for the 2024 season. The goal is to find a car that consistently delivers the highest and most reliable results across all tracks. By leveraging race data from the past three seasons (2021, 2022, and 2023), we aim to pinpoint which cars have dominated the championship overall and which performed exceptionally well on specific tracks during the 2023 season.



## Project Structure


### 1. Web Scraping
Data for the analysis was collected using web scraping techniques from the official GT World Challenge Europe website. This step involved writing and executing scripts using the **BeautifulSoup** library to extract race results, car specifications, and other relevant information for each car and race.

### 2. Data Cleaning
Following data extraction, the raw data underwent a thorough cleaning process to ensure its accuracy and usability for subsequent analysis. This involved:
- Removing duplicate entries
- Handling missing or inconsistent data
- Standardizing car names and track information to maintain uniformity across the dataset


### 3. Data Analysis
The cleaned dataset was analyzed to determine the most optimal car. The key objectives included:
- Identifying the cars that consistently performed best across the past three seasons (2021, 2022, and 2023)
- Analyzing which cars excelled on specific tracks during the 2023 season
- Compiling the results to provide a clear recommendation for the best car to use in the GT World Challenge Europe for the 2024 season.



## Methodology


### 1. Accrual of Points
Points were awarded to the top 10 finishers in each race using the following system:

- 1st place: 13 points (including 3 bonus points)
- 2nd place: 11 points (including 2 bonus points)
- 3rd place: 9 points (including 1 bonus point)
- 4th place: 7 points
- 5th place: 6 points
- 6th place: 5 points
- 7th place: 4 points
- 8th place: 3 points
- 9th place: 2 points
- 10th place: 1 point


### 2. Weighing and Normalizing Points

#### 2.1. Weighing by Race Duration
Since different tracks host races of varying lengths, points were adjusted by a coefficient proportional to the race duration:
- The base race length was defined as 50 laps.
- Points for each race were multiplied by a ratio corresponding to the race duration.
- For example, a win (13 points) in a 64-lap race would be adjusted to 16.64 points using the formula: `13 × (64 / 50) = 16.64 points`.

#### 2.2. Normalizing by Number of Races
To account for the varying number of races held at each track, total points scored by a car were divided by the number of races at that track:
- Example: If the Mercedes-AMG GT3 scored 60 points at Barcelona over 3 races, the normalized score would be `60 / 3 = 20 points`.


### 3. Identifying Leaders

#### 3.1. Leaders by Season
- Median positions were calculated for each car across all tracks for a season.
- The car with the lowest median position was designated as the season leader, indicating consistent high performance.

#### 3.2. Leaders by Specific Race Track
- Points were aggregated for each car at individual tracks.
- The car with the highest total points at a specific track was recognized as the track leader.


### 4. Data Visualization
The results were visualized to facilitate a better understanding of the analysis and to make data-driven recommendations.



## Insights


### Leaders by the Median of Medians for the 2021, 2022, and 2023 Seasons
![Leaders by the Median of Medians for the 2021, 2022, and 2023 Seasons](images/Leaders_by_the_Median_o_Medians_Seasons.png)


### Leaders by Median Position for the 2021 Season
![Leaders by median position for the 2021 season](images/Leaders_by_median_position_for_the_2021_season.png)


### Leaders by median position for the 2022 season
![Leaders by median position for the 2022 season](images/Leaders_by_median_position_for_the_2022_season.png)


### Leaders by median position for the 2023 season
![Leaders by median position for the 2023 season](images/Leaders_by_median_position_for_the_2023_season.png)


### Leaders at a specific race track for the 2023 season
![Leaders at a specific race track for the 2023 season](images/Leaders_at_a_specific_race_track_for_the_2023_season.png)



## Recommendations


### Top Recommendation: `Audi R8 LMS GT3 EVO 2`
For the 2024 season of the GT World Challenge Europe, the `Audi R8 LMS GT3 EVO 2` stands out as the top recommendation. In the 2023 season, this car achieved a stellar first place with a median finish position of 2.0, making it the most consistent performer of the year.

- **Strengths in 2023**: The `Audi R8 LMS GT3 EVO 2` dominated across various tracks, consistently securing first or second place on almost every circuit. Its exceptional performance underscores its adaptability and competitiveness in different racing conditions.
- **Weaknesses in 2023**: The only track where the `Audi R8 LMS GT3 EVO 2` struggled slightly was Barcelona,  where it barely made it into the points zone, finishing near the bottom of the standings.

Furthermore, the `Audi R8 LMS GT3 EVO 2` has been one of the top performers over the past three seasons (2021, 2022, and 2023). It achieved a median finish position of 2.0, sharing this outstanding record with the `Mercedes-AMG GT3`.


### Strong Contender: `BMW M4 GT3`
The `BMW M4 GT3` is another noteworthy option for the 2024 season. In 2023, it placed second overall, with a median finish position of 2.5, proving its potential to challenge the very best.

- **Strengths in 2023**: The `BMW M4 GT3` demonstrated exceptional performance at Monza, where it dominated with a significant margin. It also ranked first in points at Misano and Zandvoort, showcasing its ability to excel on a variety of tracks. When it wasn’t securing the top spot, the `BMW M4 GT3` consistently finished within the top three on most tracks.
- **Weaknesses in 2023**: However, its performance was notably weaker at Barcelona and Nürburgring, where it struggled to score points and barely made it into the points zone, finishing near the bottom of the standings.


### Strong Contender: `Mercedes-AMG GT3/GT3 EVO`
The `Mercedes-AMG GT3/GT3 EVO` also presents itself as a strong contender for the 2024 season. In the 2023 season, it secured a commendable third place overall, with a median finish position of 3.0.

- **Strengths in 2023**: This car demonstrated dominance at Nürburgring, where it consistently outperformed other competitors. Additionally, it led in points at Barcelona and Circuit Paul Ricard, showcasing its strength on these challenging tracks.
- **Consistency**: Even on tracks where it didn’t secure the top spot, the `Mercedes-AMG GT3/GT3 EVO` remained highly competitive, finishing within the leading group or just behind the leaders.

Over the last three seasons, the `Mercedes-AMG GT3/GT3 EVO` has shown consistent high performance, achieving a median finish position of 2.0, which places it among the elite alongside the `Audi R8 LMS GT3 EVO 2`.
