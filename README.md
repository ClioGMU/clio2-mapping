## Clio 2: Mapping assignment

Your assignment is to use the U.S. Census data in [NHGIS](https://www.nhgis.org/). Follow this process.

1. Try the sample code in `mapping-demo.Rmd`. This will use the sample data in the `census` directory and the sample shapefiles in the `shapefiles` directory.

2. Create an account at [NHGIS](https://www.nhgis.org) and [read the guide](https://www.nhgis.org/sites/www.nhgis.org/files/using_the_nhgis_data_finder.pdf) about how to use the data finder.

3. Using the [NHGIS Data Finder](https://data2.nhgis.org/main), pick a set of census data that interests you, and download it from the NHGIS. You could choose to do a comparison over time, or across variables, or in some other historically interesting way. You may use either state or county data, though generally county data is more interesting than state data. Don't go overboard in downloading lots of data at the start. Pick one thing of interest to begin, and you can always download more later. Put the data you downloaded into the same directory as this README file.

4. NHGIS provides shapefiles for each census year, but their shapefiles are much higher resolution than we need. Download simplified shapefiles that correspond to the year and geography level you need from [here](https://lincolnmullen.com/files/census-shp/). For instance, if you download 1850 manufacturing data for states, you need `US_state_1850.simplified.zip`. You will need to put those shapefiles in the same directory as the data you downloaded. But you will also need unzip those files. If you do that correctly, you will end up with a directory called `US_state_1850.simplified/` with four files named like this: `US_state_1850.simplified.shp`.

4. Explore the data. Use the codebooks to understand the variables' meaning. For instance, the column `ADQ001` in one of the sample CSV files has the total population, while `ADZ001` has the population in towns over 2,500 people. It is a good idea to explore the data using the techniques we learned for exploratory data analysis, including histograms and bar charts.

5. Make maps of the data. To do this, you will need to join the census data to the spatial data. The maps can be either interactive (with leaflet) or static (with ggplot2).

6. As an advanced step, try normalizing the data in the maps by population or by area.

7. Finally, clean up what you have done and put it into a form that a normal historian could read. Delete visualizations that were not useful. Surround the maps that you keep with explanatory prose. Include a minimum of two maps (interactive or static) and approximately 500 words of prose. You may also include non-map visualizations if they are usefu to you. The prose and maps should combine to make some historically meaningful interpretation using the census data. Include the code blocks, which should contain only the code necessary to generate the figures. Turn in the HTML file that you created.
