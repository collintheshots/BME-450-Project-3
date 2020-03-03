# BME 450 Project 3 SeisMap
Collin Tasaka

Winter 2020

This class has been very difficult for me and my lack of coding experience has put me at a disadvantage. The only other coding class I have taken was your Matlab class, which I also did not learn much in. While I am really enjoying the content, lectures, and tests, the projects are very hard. I can figure them out, but it takes me far more time than others. I hope that this project shows what I have learned.

I got my data by going to the USGS Earthquake Catalog and selecting earthquakes magnitude 2.5 and above from 2010 to today within a certain boundary. The boundary I chose was the same as the one that you approved for the class from Matthew, (-131.821, -122.1706, 38.8915, 52.013). This creates a bounding box around the plate of Juan de Fuca. I had originally chosen the larger area described in your project description, but it was ultimately too much data and it took 10 minutes to produce each of my graphs.

I used some aspects of previous projects to properly import my data into jupyter notebook from the GitHub urls. This was done using Pandas to read and grab data from my csv files on GitHub. I needed to read the time, magnitude, latitude, and longitude data from the imported USGS csv files. Then, after importing the Matlab plotting library (matplotlib), I was able to graph the earthquake magnitude vs time during this 2010 to now time period.

