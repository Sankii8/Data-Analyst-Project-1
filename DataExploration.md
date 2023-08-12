Link To the DATASET- https://ourworldindata.org/
                     https://ourworldindata.org/covid-deaths
                     https://ourworldindata.org/covid-vaccinations



# Data-Analyst-Projects
Project 1 : Data Exploration using Sql 

This code is an SQL script that performs data exploration and analysis on COVID-19 data, specifically related to cases, deaths, population, and vaccinations. It 
employs various SQL techniques such as joins, Common Table Expressions (CTEs), temporary tables, window functions, aggregate functions, creating views, and 
converting data types to derive meaningful insights from the COVID-19 dataset.

Here's a breakdown of the different parts of the code and their purposes:

Initial Data Retrieval:
The script begins by retrieving raw COVID-19 data from a table named CovidDeaths in a database schema named PortfolioProject. It selects specific columns 
(Location, date, total_cases, new_cases, total_deaths, population) from the table for countries where the continent is not null. The data is ordered by location 
and date.

Calculating Death Percentage:
The script calculates the death percentage for each location (country) by dividing the total deaths by total cases and multiplying by 100. This provides an 
estimate of the likelihood of dying if contracting COVID-19 in each country. The results are ordered by location and date.

Calculating Percentage of Population Infected:
The script calculates the percentage of the population infected with COVID-19 in each location by dividing total cases by the population and multiplying by 100. 
This helps understand the scale of infection within each country. The results are ordered by location and date.

Countries with Highest Infection Rate:
This query identifies countries with the highest infection rates compared to their population. It groups the data by location and population, calculating the 
maximum infection count and the corresponding percentage of population infected. The results are ordered by the percentage of population infected in descending 
order.

Countries with Highest Death Count:
This query identifies countries with the highest total death counts. It groups the data by location and calculates the maximum total death count for each country. 
The results are ordered by the total death count in descending order.

Breaking Down by Continent - Death Count:
This query groups the data by continent and calculates the maximum total death count for each continent. The results provide insights into continents with the 
highest death counts. The results are ordered by the total death count in descending order.

Global COVID-19 Numbers:
This query calculates global COVID-19 statistics, including total cases, total deaths, and the death percentage. The data is aggregated across all locations and 
ordered by date.

Total Population vs Vaccinations:
This query combines COVID-19 deaths data with vaccination data. It calculates the rolling sum of new vaccinations per location and displays the percentage of the 
population that has received at least one COVID-19 vaccine. The results are ordered by location and date.

Using CTE for Vaccination Calculation:
This section rewrites the previous query using a Common Table Expression (CTE) to perform the rolling vaccination calculation.

Using Temporary Table for Vaccination Calculation:
This section rewrites the previous query using a temporary table to perform the rolling vaccination calculation.

Creating a View for Visualization:
The script creates a view named PercentPopulationVaccinated that encapsulates the logic for calculating the rolling vaccination data. This view can be used later 
for data visualization purposes.

Overall, this script leverages SQL queries and techniques to analyze COVID-19 data, calculate relevant metrics, and prepare the data for potential visualization. 
It's likely part of a larger data analysis or reporting project related to the COVID-19 pandemic.
