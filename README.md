Assignment
This Python script utilizes Apache Spark and Folium to analyze and visualize earthquake data. Here's a breakdown of what the script does:

Data Ingestion: The script reads earthquake data from a CSV file "database.csv" using Apache Spark's DataFrame API.

Data Preparation:

Concatenates the "Date" and "Time" columns to create a new "Timestamp" column.
Converts the "Timestamp" column to the appropriate format.
Casts columns to their correct data types (Magnitude, Latitude, Longitude, Depth).
Filters the dataset to consider earthquakes with a magnitude greater than or equal to 5.0.
Data Analysis:

Calculates the average depth and magnitude of earthquakes grouped by their type.
Classification:

Defines a function to categorize earthquakes based on their magnitude into three categories: "Low", "Moderate", and "High".
Geospatial Analysis and Visualization:

Calculates the distance of each earthquake from the reference point (0,0).
Visualizes earthquake locations on an interactive map using Folium, with each marker representing an earthquake. The map is saved as "map.html".
Data Export:

Converts the Spark DataFrame to a Pandas DataFrame for easier export.
Saves the final processed data to CSV format as "final_data.csv".
Dependencies
Python 3.x
Apache Spark
Folium
Pandas
Instructions
Ensure all dependencies are installed.
Place the earthquake data CSV file ("database.csv") in the same directory as the script.
Run the script.
The processed data will be saved as "final_data.csv", and the interactive map will be saved as "map.html" in the same directory.
Note
Make sure to adjust file paths or configurations as needed based on your environment.
The script assumes a reference point of (0,0) for geospatial analysis.
