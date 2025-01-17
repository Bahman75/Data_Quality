# Boston Crime Data Analysis and Visualization
![image](https://github.com/user-attachments/assets/4c660f5d-7ebc-41a9-b8e0-cd68208f0965)

This repository contains the analysis and visualization of the Boston Crime dataset, focusing on cleaning, transforming, and integrating data for geospatial and temporal insights. The project applies advanced data preprocessing techniques and geospatial mapping to uncover meaningful trends in crime data.

## Features

- **Data Cleaning**: 
  - Removed duplicates to ensure data accuracy.
  - Handled missing values using imputation techniques for critical columns like `Lat` and `Long`.
  - Standardized formats for consistency.

- **Data Transformation**:
  - Split complex columns (e.g., `OCCURRED_ON_DATE`) into individual components (`YEAR`, `MONTH`, `DAY`, `TIME`) for enhanced analysis.
  - Merged offense code details with the crime dataset using `OFFENSE_CODE`, retaining only the `DESCRIPTION` column.

- **Visualization**:
  - Interactive geospatial map using Plotly to visualize crime trends over time and location.
  - Summary statistics and insights generated through automated reporting tools like Sweetviz.

## Data Overview

- **CRIME Dataset**: Contains detailed records of crime incidents, including time, location, and type of offense.
- **OFFENSE_CODES Dataset**: Provides descriptions and classifications of offense codes.

### Key Columns:
- `INCIDENT_NUMBER`: Unique identifier for each crime event.
- `OFFENSE_CODE`: Numeric code representing the type of offense.
- `DESCRIPTION`: Detailed offense description (merged from offense codes).
- `OCCURRED_ON_DATE`: Timestamp of the crime incident.
- `Lat` & `Long`: Geographic coordinates of the crime location.
- `YEAR`, `MONTH`, `DAY_OF_WEEK`, `HOUR`: Time attributes for temporal analysis.

## Tools and Technologies

- **Python Libraries**: Pandas, NumPy, Plotly, Sweetviz, Matplotlib
- **Geospatial Mapping**: Plotly's Scatter Mapbox
- **Data Transformation**: Pandas for cleaning, merging, and transforming datasets.

## How to Use

1. Clone the repository:  
   ```bash
   git clone https://github.com/MiladRamezani0/boston-crime-analysis.git
   ```
2. Install the required libraries:  
   ```bash
   pip install -r requirements.txt
   ```
3. Run the analysis script to generate visualizations and insights:  
   ```bash
   python analysis.py
   ```

## Visualizations

- **Interactive Geospatial Map**: Highlights crime locations by type and time.
- **Temporal Analysis**: Trends over years, months, and days of the week.

## Future Work

- Enhancing predictive analysis for crime hotspots.
- Integration of additional datasets for deeper insights.

## Contributors

- **Milad Ramezani Ziarani**  
  - LinkedIn: [Milad Ramezani Ziarani](https://www.linkedin.com/in/milad-ramezani-ziarani-299b23100)  
  - GitHub: [MiladRamezani0](https://github.com/MiladRamezani0)
- **Bahman Amirsardary**  
  - LinkedIn: [Bahman Amirsardary](https://www.linkedin.com/in/bahman-amirsardary-3405b8132/)  
  - GitHub: [BahmanAmirsardary](https://github.com/Bahman75)

## License

This project is licensed under the [MIT License](LICENSE).
