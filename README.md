# NYC-Open-Data

## Packages
* matplotlib
* pandas
* geopandas
* descartes
* sodapy
* shapely


## Datasets
Shapefiles are accessible via [Berkeley Library Geodata](https://geodata.lib.berkeley.edu/)
NYC data are accessible via [NYC Open Data](https://opendata.cityofnewyork.us/data/)

## Plot NYC Buildings as Background
To retrieve NYC buildings, download [NYC building shapefile](https://dev.socrata.com/foundry/data.cityofnewyork.us/e42i-6hpb) from [Berkeley Library Geodata](https://geodata.lib.berkeley.edu/). 
```
buildings = gpd.read_file('./shapefile/geo_export_426d25b7-267f-47a3-88cc-132bf267b23d.shp')
fig, ax = plt.subplots(figsize = (15, 15))
buildings.plot(ax=ax)
```
![download](https://user-images.githubusercontent.com/79494397/207496710-7d4402a9-b10b-4e64-af7f-beab311a19b0.png)

## Plot NYC Streets as Background
To retrieve NYC streets, download [NYC roads shapefile](https://geodata.lib.berkeley.edu/catalog/nyu-2451-34499) from [Berkeley Library Geodata](https://geodata.lib.berkeley.edu/).
```
roads = gpd.read_file('./shapefile/geo_export_426d25b7-267f-47a3-88cc-132bf267b23d.shp')
fig, ax = plt.subplots(figsize = (15, 15))
roads.plot(ax=ax)
```
![download](https://user-images.githubusercontent.com/79494397/207496905-ccb6f122-4b0a-4d4f-b4ee-f6f3dd36910c.png)

## Plot NYC Subway Routes as Background
To retrieve NYC subway routes, download [NYC subway routes shapefile](https://geodata.lib.berkeley.edu/catalog/nyu-2451-34758) from [Berkeley Library Geodata](https://geodata.lib.berkeley.edu/).
```
subway_routes = gpd.read_file('./shapefile/geo_export_426d25b7-267f-47a3-88cc-132bf267b23d.shp')
fig, ax = plt.subplots(figsize = (15, 15))
subway_routes.plot(ax=ax)
```
