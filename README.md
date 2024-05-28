# CO2 Emissions Visualization with Folium

This project explores CO2 emissions per capita data from the World Development Indicators Dataset using the Folium library. Folium allows us to create interactive maps with geographic overlays for data visualization.

## Data Source

* World Development Indicators Dataset (compressed with bz2)
* World Countries GeoJSON file (`data/world-countries.json`)

## Libraries Used

* folium
* pandas
* warnings

## Script Overview

1. **Import Libraries:** Import necessary libraries (`folium`, `pandas`, and `warnings`).
2. **Load Geo Data:** Load the world countries GeoJSON file (`data/world-countries.json`).
3. **Read World Development Indicators:** Read the World Development Indicators data from a compressed CSV file (`data/Indicators.bz2`).
4. **Data Selection:** Select data for CO2 emissions per capita in the year 2011.
5. **Data Preparation:** Create a DataFrame containing country codes and CO2 emission values for plotting.
6. **Map Creation:** Initialize a Folium map with a high-level zoom.
7. **Choropleth Visualization:** Create a choropleth map using Folium, binding the prepared DataFrame with the GeoJSON data. The map displays CO2 emissions per capita with color variations.
8. **Save Interactive Map:** Save the Folium map as an HTML file (`saved_info/plot_data.html`).
9. **Display Interactive Map (Optional):** Utilize IPython.display to display the saved HTML file within a Jupyter notebook (for a preview of the interactive map).

## Running the Script

1. Save the script as a Python file (e.g., `USING FOLIUM LIBRARY FOR GEOGRAPHIC OVERLAYS.ipynb`).
2. Ensure you have the required libraries installed (`folium`, `pandas`). You can install them using `pip install folium pandas`.
3. Place the World Development Indicators data (`data/Indicators.bz2`) and the world countries GeoJSON file (`data/world-countries.json`) in the same directory as your script.
4. Run the script from the command line: `python USING FOLIUM LIBRARY FOR GEOGRAPHIC OVERLAYS.ipynb`.
5. This will generate the HTML file (`saved_info/plot_data.html`) containing the interactive map. You can open this file in a web browser to explore the CO2 emissions data visually.

## Additional Notes

* The script utilizes warnings filters to avoid unnecessary warnings during execution.
* The IPython.display import is for showcasing the interactive map within a Jupyter Notebook. You can comment it out if not using a Jupyter environment.

This project demonstrates a basic example of using Folium to visualize data with geographic overlays. You can further explore this library to create more complex and informative maps.
