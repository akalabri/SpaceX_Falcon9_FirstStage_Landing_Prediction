# SpaceX Launch Data Analysis

## Overview

In this capstone assignment, we will be working with SpaceX launch data gathered from the SpaceX REST API. The API provides information about SpaceX launches, including details about the rocket used, payload delivered, launch and landing specifications, and landing outcomes. Our goal is to use this data to predict whether SpaceX will attempt to land a rocket or not.

We will work with the SpaceX REST API, specifically the `/launches/past` endpoint, to obtain past launch data. This data is retrieved using a GET request and is returned in JSON format, which contains a list of JSON objects, each representing a launch.

To analyze and visualize this data effectively, we will convert the JSON data into a pandas DataFrame using the `json_normalize` function. This will allow us to work with structured data in a tabular form.

Additionally, we will explore an alternative data source for Falcon 9 launch data by web scraping relevant Wiki pages using the Python BeautifulSoup package. We will parse the HTML tables, convert the data into a pandas DataFrame, and clean the dataset for further analysis.

## Data Transformation and Wrangling

### API Data Transformation

- We will obtain detailed data for specific attributes such as Booster, Launchpad, Payload, and Core by targeting relevant API endpoints.
- Some columns contain identification numbers rather than actual data, and we will use the API to gather specific data for each ID number.

### Filtering Falcon 1 Launches

- The dataset obtained from the API includes data for the Falcon 1 booster, which we want to exclude. We will filter or sample the data to remove Falcon 1 launches.

### Handling Null Values

- Some columns may contain NULL (missing) values, which need to be addressed for meaningful analysis.
- Specifically, we will focus on the `PayloadMass` column, calculate the mean of the non-null values, and replace NULL values with the calculated mean.
- The `LandingPad` column with NULL values will be left as is, as it indicates the absence of a landing pad.

## Future Analysis

With a clean and well-structured dataset, we can perform various analyses and visualizations to gain insights into SpaceX launches. Potential future steps include:

- Exploring the relationship between payload mass and launch success.
- Analyzing the impact of different boosters on the success of landings.
- Visualizing launch and landing outcomes over time.
- Using one-hot encoding to handle categorical data, such as the presence or absence of a landing pad.

By leveraging both API data and web scraping, we can create a comprehensive dataset for insightful analysis of SpaceX launch data.

## Data Sources

- [SpaceX REST API](https://api.spacexdata.com/v4/launches/past)
- Web scraping of relevant Wiki pages for Falcon 9 launch records.

## Technologies Used

- Python
- Requests library for API data retrieval
- BeautifulSoup for web scraping
- Pandas for data manipulation and analysis
- Matplotlib and Seaborn for data visualization

## Author

[Aflah Al Abri]

## License

This project is licensed under the [MIT License](LICENSE.md).
