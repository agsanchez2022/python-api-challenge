# **WeatherPy and VacationPy**

## **Part 1: WeatherPy**

In this deliverable, you'll create a Python script to visualize the weather of over 500 cities of varying distances from the equator. You'll use the **citipy** Python library, the **OpenWeatherMap API**, and your problem-solving skills to create a representative model of weather across cities.

For this part, you'll use the `WeatherPy.ipynb` Jupyter notebook provided in the starter code ZIP file. The starter code will guide you through the process of using your Python coding skills to develop a solution to address the required functionalities.

### **Requirement 1: Create Plots to Showcase the Relationship Between Weather Variables and Latitude**

To fulfill the first requirement, you'll use the **OpenWeatherMap API** to retrieve weather data from the cities list generated in the starter code. Next, you'll create a series of scatter plots to showcase the following relationships:

- **Latitude vs. Temperature**
- **Latitude vs. Humidity**
- **Latitude vs. Cloudiness**
- **Latitude vs. Wind Speed**

### **Requirement 2: Compute Linear Regression for Each Relationship**

To fulfill the second requirement, compute the linear regression for each relationship. Separate the plots into **Northern Hemisphere** (greater than or equal to 0 degrees latitude) and **Southern Hemisphere** (less than 0 degrees latitude). You may find it helpful to define a function in order to create the linear regression plots.

Next, create a series of scatter plots. Be sure to include:

- The **linear regression line**
- The **model's formula**
- The **r² values**

You should create the following plots:

- **Northern Hemisphere: Temperature vs. Latitude**
- **Southern Hemisphere: Temperature vs. Latitude**
- **Northern Hemisphere: Humidity vs. Latitude**
- **Southern Hemisphere: Humidity vs. Latitude**
- **Northern Hemisphere: Cloudiness vs. Latitude**
- **Southern Hemisphere: Cloudiness vs. Latitude**
- **Northern Hemisphere: Wind Speed vs. Latitude**
- **Southern Hemisphere: Wind Speed vs. Latitude**

After each pair of plots, explain what the linear regression is modeling. Describe any relationships that you notice and any other findings you may uncover.

## **Part 2: VacationPy**

In this deliverable, you'll use your weather data skills to plan future vacations. You'll also use Jupyter notebooks, the **geoViews** Python library, and the **Geoapify API**.

The code needed to import the required libraries and load the CSV file with the weather and coordinates data for each city created in Part 1 is provided to help you get started.

Your main tasks will be to use the **Geoapify API** and the **geoViews** Python library and employ your Python skills to create map visualizations.

### **Steps:**

1. **Create a map** that displays a point for every city in the `city_data_df` DataFrame. The size of the point should represent the humidity in each city.

2. **Narrow down the `city_data_df` DataFrame** to find your ideal weather conditions. For example:
   - A max temperature lower than 27 degrees but higher than 21
   - Wind speed less than 4.5 m/s
   - Zero cloudiness

   *Note: Feel free to adjust your specifications, but make sure to set a reasonable limit to the number of rows returned by your API requests.*

3. **Create a new DataFrame called `hotel_df`** to store the city, country, coordinates, and humidity.

4. For each city, use the **Geoapify API** to find the first hotel located within 10,000 meters of your coordinates.

5. **Add the hotel name and the country** as additional information in the hover message for each city on the map.
