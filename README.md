# BME 450 Project 3 SeisMap
Collin Tasaka

Winter 2020

This class has been very difficult for me and my lack of coding experience has put me at a disadvantage. The only other coding class I have taken was your Matlab class, which I also did not learn much in. While I am really enjoying the content, lectures, and tests, the projects are very hard. I can figure them out, but it takes me far more time than others. I hope that this project shows what I have learned.

I got my data by going to the USGS Earthquake Catalog and selecting earthquakes magnitude 2.5 and above from 2010 to today within a certain boundary. The boundary I chose was the same as the one that you approved for the class from Matthew, (-131.821, -122.1706, 38.8915, 52.013). This creates a bounding box around the plate of Juan de Fuca. I had originally chosen the larger area described in your project description, but it was ultimately too much data and it took 10 minutes to produce each of my graphs.

I used some aspects of previous projects to properly import my data into jupyter notebook from the GitHub urls. This was done using Pandas to read and grab data from my csv files on GitHub. I needed to read the time, magnitude, latitude, and longitude data from the imported USGS csv files. Then, after importing the Matlab plotting library (matplotlib), I was able to graph the earthquake magnitude vs time during this 2010 to now time period.

![Magnitude vs Time](https://github.com/collintheshots/BME-450-Project-3/blob/master/magvstime.png?raw=true)

This data shows that there weren't many earthquakes greater than 6 and none above 7 during this time period in this region.

Then, I had to find a way to graph the data points on a map. Luckily, an online source had already done that and I followed their instructions and got a map of the region I selected on Open Street Map. I was then able to read the file and plot. The key to getting the datapoints into different sizes and colors is the for loop with if statements. It reads the magnitude of each data point and if the magnitude is bigger than a certain number, then it plots the points with my chosen point size and color. Transparency can be adjusted as well.

![forifelse](https://github.com/collintheshots/BME-450-Project-3/blob/master/forifelse.png?raw=true)

The result of this code is the colorful map of the selected region. 

![Plotting SeisMap](https://github.com/collintheshots/BME-450-Project-3/blob/master/Seismic%20Plot.png?raw=true)

Across what geographic area are you able to observe earthquake data in this map? Why do you see most of the earthquakes in that area? 

The bounding box we drew was meant to encompass the Juan de Fuca Plate. This is apparent because we can see on the graph I created the distinct Blanco Fracture Zone and Gorda Ridge.

![Juan de Fuca](https://github.com/collintheshots/BME-450-Project-3/blob/master/Page_092_Figure_1-1.jpg?raw=true)

We see a lot of earthquakes in this area because the Juan de Fuca plate is subducting underneath the North American plate in the Cascadia Subduction Zone. This means that as the Juan de Fuca plate slides into the mantle, it catches on the North American plate and builds up pressure which is released in the form of earthquakes.

What is the range of earthquake size (magnitude) in these data? What is the average earthquake size in this area?

We can see that the earthquakes range from very small up to 6.5 during this time period. Our data has been bounded to 2.5 at the lower end, as set per instructions from the USGS earthquake catalog. The average earthquake magnitude is 3.24

![maxminmean](https://github.com/collintheshots/BME-450-Project-3/blob/master/magnitudeearth.png?raw=true)

Map the earthquakes in April 2015(include this map in your report). Where are those earthquakes mostly located? What event can you link these earthquakes to? 

![SeisMap April 2015](https://github.com/collintheshots/BME-450-Project-3/blob/master/apr2015quakes.png?raw=true)

Most of these earthquakes are located on the southern end of the Juan de Fuca Plate. This is due to the eruption of Axial Seamount on April 23rd, 2015, around 2230. The eruption created a release of earthquakes in the region.

![Axial Seamount](https://github.com/collintheshots/BME-450-Project-3/blob/master/300px-WestcoastSeaplates.svg.png?raw=true)


