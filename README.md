# GeoJSON of Saudi Arabia Regions
A script that builds a GeoJSON of Saudi Arabia goveranates with an demostration

## Motivation
I wanted to create a heatmap of Saudi Arabia such that the variation in color is indicated by the data point in my dataset, such as the example picture below

![alt text](https://www.researchgate.net/profile/Hala_Elmorshedy/publication/282947082/figure/fig7/AS:285973712785414@1445192854943/Kingdom-of-Saudi-Arabia-map-showing-the-13-provinces-From-mapsopensourcecom_Q320.jpg)

Such visualization requires us to know the latitude and longitude of every point on the boundaries of each region. In other words we need the exact geographic encoding of the regions, which we call [GeoJson](http://www.GeoJson.org).

One way to do that is by manually drawing the boundaries using tools such as [geojson.io](http://www.geojson.io), and exporting the GeoJSON data. An easier way is to utilize OpenStreetMaps to obtain that data. 

In this repo I wrote a script that queries the GeoJson data of all regions of Saudi, and demonstrated it on the map using `folium` visualization library.

Note: github doesn't render `folium` maps, so please [click here](https://github.com/wjdanalharthi/GeoJSON-of-Saudi-Arabia-Regions/blob/master/example/SA_regions_map.html) or [here](https://nbviewer.jupyter.org/github/wjdanalharthi/GeoJSON-of-Saudi-Arabia-Regions/blob/master/example/SA_regions_vis.ipynb) to see the map


## How to use it
By executing the python code in [SA_regions_geojsons_builder.py](https://github.com/wjdanalharthi/GeoJSON-of-Saudi-Arabia-Regions/blob/master/SA_regions_geojsons_builder.py), the JSON file [SA_regions.json](https://github.com/wjdanalharthi/GeoJSON-of-Saudi-Arabia-Regions/blob/master/data/SA_regions.json)  will be created, and can be fed into heatmap visualizations libraries such as folium as demonstrated in [SA_regions_vis.ipynb](https://github.com/wjdanalharthi/GeoJSON-of-Saudi-Arabia-Regions/blob/master/example/SA_regions_vis.ipynb)


To reuse this code for another country, modify the names and OSM codes in the python script and rerun it
 
