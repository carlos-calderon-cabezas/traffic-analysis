# Traffic Data Analysis and Predictions

![image](https://github.com/user-attachments/assets/45336690-769a-4dec-a385-a87ede89dd79)

[**Click here for the spanish version**](https://github.com/carlos-calderon-cabezas/traffic-analysis/blob/main/README.md)

## Table of Contents

- [Project Description](#project-description)
- [Project Content](#project-content)
- [Usage Instructions](#usage-instructions)
- [Brief Summary of Conclusions and Recommendations](#brief-summary-of-conclusions-and-recommendations)

## Project Description

This project is a brief and simple demonstration of traffic data analysis and predictions that I used to perform for a major company in Ecuador, dedicated to the study, planning, and construction of road infrastructure projects. In this specific case, it involved the expansion of a road.

Due to the company's confidentiality policies regarding project data, I cannot include all the parameters obtained by this sensor, nor all the variables that were part of the study, nor provide the exact location of the study. Additionally, part of the data shown here has been intentionally modified.

This project uses traffic data collected from measurements taken between August 2, 2021, and October 12, 2021, totaling 71 consecutive days.

To conduct the project, a traffic sensor was placed at a strategic point on the road, capable of counting passing vehicles and detecting characteristics such as vehicle type, speed, and the date and time they passed. In the dataset corresponding to the traffic sensor (*sensor_df*), each row represents the hourly vehicle count by type, their average speed, and their 85th percentile speed.

Additionally, there is a dataset corresponding to the weather conditions at the time the traffic data was collected. These data were also recorded hourly for each of the 71 days of traffic measurements. Historical weather data from different parts of the world can be obtained from [Visual Crossing](https://www.visualcrossing.com/weather/weather-data-services).

The project analyzes data such as the number of vehicles passing at a certain hour or the days of the week with the most vehicles of a certain type, among other aspects.

In the predictive analysis of this project, the behavior of the traffic flow influenced by the day of the week, the hour, and the current weather conditions is studied.

## Project Content

- `Traffic_analysis.ipynb`: Google Colab Jupyter Notebook written in Python.
- `input` folder with the following input datasets:
   - `norte_sur_df.csv` dataset with traffic measurements taken with a *MetroCount RoadPod VT* traffic sensor.
   - `weather_df.csv` dataset with historical weather data collected during the traffic measurement period.

## Usage Instructions

To use this project, follow these steps:

1. Clone the repository or download all files.
2. Ensure you have the necessary dependencies installed, such as Jupyter Notebook and the Python libraries used in the notebooks, including *pandas*, *matplotlib*, and *seaborn*.
3. Open the `Traffic_analysis.ipynb` file in Jupyter Notebook or JupyterLab.
4. Run the notebook cells to see the analyses and predictions.

No additional software installation or environment configuration is needed beyond having Jupyter and the previously mentioned Python libraries.

## Brief Summary of Conclusions and Recommendations

- A histogram was created to analyze average speed, revealing that the majority of vehicles travel between 65 and 75 kilometers per hour. Since the traffic sensor is located in an urban area with a speed limit of 50 km/h, it is recommended to install speed bumps in the town center and request the traffic authority to install a speed radar to ticket drivers who do not respect the limit.
- A considerable volume of heavy traffic was observed during the early hours, especially between 11 PM and 3 AM. It is recommended to request the traffic authority to keep the traffic light operational 24 hours a day since it currently turns off between midnight and 5 AM. This will enhance safety, especially for pedestrians and vehicles crossing side streets, and potentially reduce the number of accidents.
- A brief study of potential toll revenue for the new toll station planned by the concessionaire was conducted. Given the heavy vehicle traffic and the high toll rates for these vehicles, an estimated monthly revenue of USD 320,000 is expected. It is recommended that the concessionaire use the collected funds to maintain the road surface and traffic signs in optimal condition to encourage drivers to choose this route over alternative routes.
- A predictive analysis of the vehicle fleet was performed to predict the maximum traffic flow for the next 30 years, analyzing several additional variables, including the country's economic indices and vehicle fleet growth. An estimated heavy vehicle flow of approximately 15,000 heavy vehicles per day after 30 years is expected. However, due to project confidentiality, detailed study results cannot be shown.
  - This predictive model allowed the concessionaire to recommend expanding the existing road from one lane per direction to three lanes per direction, meeting certain parameters for material procurement, machinery, the number of excavations needed per section, and the construction techniques to be employed.
