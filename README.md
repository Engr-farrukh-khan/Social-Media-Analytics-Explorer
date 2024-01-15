# Visual Explorer

## Contributors
Gia Khang Ngo (Laru27), Han Lin (hanslin2014), Pawan Nihure (pawan-nihure), Hemit Dedhia (hemit-dedhia)

## Introduction
The Visual Explorer is a Streamlit web application that analyzes social media user statistics from different regions. The project is contributed by Gia Khang Ngo.

## Raw Data Display
Raw data is imported from multiple data CSV files  using Pandas and displayed using Streamlit. The raw data is presented in an expandable section for users to inspect.

## Download Raw Data
Users can download the raw Twitter data in CSV format using a download button.

## Sidebar
The sidebar allows users to input features for analysis, specifically selecting regions and social media platforms. Multiselect widgets are used for user input.

## Map Visualization
A map is displayed using the PyDeck library, showing the number of social media users per region. Hexagon layers are used to visualize the distribution of users, with elevation representing the number of Twitter followers. Users can select regions from the sidebar, and the map dynamically updates.

## Web Scraping
The code includes web scraping using BeautifulSoup and requests to extract country location data from a Google Developers webpage (`https://developers.google.com/public-data/docs/canonical/countries_csv`). Extracted data is written to a CSV file (`country_loc.csv`).

### Tools and Techniques
- **Streamlit:** Used for creating the web application with interactive widgets for user input and dynamic content updates.
- **Pandas:** Utilized for data manipulation and displaying raw data.
- **PyDeck:** Employed for creating interactive and visually appealing map visualizations.
- **BeautifulSoup and requests:** Used for web scraping to extract country location data from a specified URL.

### Additional Notes
- The code assumes that the user has already cleaned Twitter data in a CSV file (`cleaned_data_Twitter.csv`).
- The map visualization dynamically updates based on user input for regions and displays the number of Twitter users in each selected region.
- Handle potential errors, such as if the user doesn't select any region in the sidebar or if the web scraping process fails. Additionally, include appropriate error messages or feedback for users.
