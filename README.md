# Country and Continent Information Program

This program is designed to provide information about countries and continents based on data imported from CSV files. It allows users to explore various aspects of countries such as population, area, endangered species, and population density. The program is menu-driven, interactive, and user-friendly.

## Summary

The program imports three CSV files: "Country_Data.csv," "Population_Data.csv," and "Threatened_Species.csv," each with 3 columns and 50 rows. These files contain essential data about countries, their populations, and threatened species.

Upon running the program, the user is presented with the following options:
1. Explore information about countries
2. Explore information about continents
3. Exit the program

The user can input their choice using numbers '1,' '2,' or '3.' Invalid inputs will prompt the user to re-enter a valid choice.

### Countries
If the user chooses to explore information about countries, they are asked to specify the country they want to learn about. The input is not case-sensitive and will be reiterated until a valid country name is entered. The program then displays general information about the selected country, such as its name, region, sub-region, and area.

#### Options Available:
1. Display a graph of the country's population from 2000 to 2020
   - The program extracts population data from "Population_Data.csv" for the selected country and plots it on a graph over the years 2000-2020.
2. Display a bar graph of threatened species for the country
   - Using data from "Threatened_Species.csv," the program generates a bar graph showing the number of threatened species categories.
3. Calculate and output the population density for a specific year chosen by the user
   - The user selects a year, and the program calculates the population density using data from "Population_Data.csv" and "Country_Data.csv."
4. Return to the main menu

After each execution, the menu is displayed until the user chooses to return to the main menu.

### Continents
Choosing to explore information about continents prompts the user to specify the continent they want to learn about. The input is not case-sensitive and will be reiterated until a valid continent name is entered. The program then displays general information about the selected continent, such as the number of countries within it.

#### Options Available:
1. Calculate and display the largest and smallest countries within the continent
   - The program calculates the largest and smallest countries by landmass using data from "Country_Data.csv."
2. Display the total area of the continent
   - By summing up the areas of countries within the continent, the program calculates and displays the total area.
3. Calculate and display countries with the highest and lowest populations for a specific year
   - The user selects a year, and the program finds countries with the highest and lowest populations using data from "Population_Data.csv."
4. Return to the main menu

The menu is displayed after each execution until the user chooses to return to the main menu.

### Functionality
- Data imports are handled within the functions.
- The program consists of three main functions: `main()`, `country()`, and `continent()`.
- Required libraries such as NumPy and Matplotlib are imported to support data processing and visualization.
- User inputs are validated to ensure correct interactions with the program.
- The program meets the specified requirements outlined in the project handout.
