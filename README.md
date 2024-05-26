# vessel-proximity

## Data Exploration

I began by studying the data given and converted the data to the required format. I eliminated timestamps with only one vessel recorded, which reduced the number of data points to ~3000. I then proceeded to build an animation using ```matplotlib``` to show the changing values of latitude and longitude sorted in increasing order of timestamps. I observed the movement of the vessels as time progressed.

## Proximity Calculation

I used the ```scikit-learn``` library function ```haversine_distances``` which calculates Haversine distances between all pairs of points in two given arrays, and mapped this distance to the cross product of the dataframe with itself. I used vectorization extensively while performing these operations. Finally, I used a group operation to get the list of MMSIs within threshold distance of each vehicle for a given timestamp.

## Learnings

I learned a lot about data exploration using Pandas while making this project. This project gave me a chance to work with geospatial data for the first time, which gave me a lot of insight on how geospatial applications work. I also realized the importance of cleaning up data before processing and how much time it can save.

## Possible Improvements

- Usage of libraries like Geopandas to deal with the geospatial data more efficiently
- Increasing efficiency of operations by using data structures such as KD trees
