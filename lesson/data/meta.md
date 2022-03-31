# Data source and wrangling process

Data downloaded from (May 14, 2019):

`https://www.census.gov/geographies/mapping-files/time-series/geo/carto-boundary-file.html`


Counties file cb_2018_us_county_20m.shp converted to GeoJSON using Mapshaper:

`mapshaper cb_2018_us_county_20m.shp -simplify 15% keep-shapes -filter-fields NAME,GEOID,STATEFP -verbose -o format=geojson precision=.00001 cb_2018_us_county.json`

Counties GeoJSON merged into states.json:

`mapshaper cb_2018_us_county.json -dissolve STATEFP -0 states.shp`

Counties GeoJSON converted to topojson:

`mapshaper cb_2018_us_county.json -o format=topojson counties.json`