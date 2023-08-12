Covid 19 Data Exploration 

Skills used: Joins, CTE's, Temp Tables, Windows Functions, Aggregate Functions, Creating Views, Converting Data Types

Data Exploration Question/Steps That have been solved through out the project refer (Data Exploration.sql)

1)Select Data that we are going to be starting with (CovidDeath from PortfolioProject File)

2)Total Cases vs Total Deaths, Shows likelihood of dying if you contract covid in your country
(select location,date,total cases,total deaths then calculate Death percentage where Locations are States And Continent is not NULL)

3)Total Cases vs Population, Shows what percentage of population infected with Covid

4)Countries with Highest Infection Rate compared to Population(Used MAX Function)

5)Countries with Highest Death Count per Population(Used Cast Funtion)

6)BREAKING THINGS DOWN BY CONTINENT - Showing contintents with the highest death count per population(Use Group By Function)

7)GLOBAL NUMBERS (Used SUM function)

8)Total Population vs Vaccinations, Shows Percentage of Population that has recieved at least one Covid Vaccine (Used CONVERT and JOIN functions)

9) Using CTE to perform Calculation on Partition By in previous query

10)Using Temp Table to perform Calculation on Partition By in previous query

11)Insert that into #PercentPopulationVaccinated

12) Creating View to store data for later visualizations

