# D3JS: Translating and Transforming GeoJSON data
[D3JS](http://d3js.org/) is a JavaScript library for creating data-visualizations for the web. It features powerful [mapping funcitonalities](https://github.com/mbostock/d3/wiki/API-Reference#d3geo-geography) that let the user create web-maps in projections other than the [Web-Mercator](http://spatialreference.org/ref/sr-org/epsg3857-wgs84-web-mercator-auxiliary-sphere/). D3 also allows for interactivity and animation, both of which are not covered here but will be in a following tutorial. 

One of the problems of working with geospatial data a la cart and D3JS are appropriately scaling and translating data. The following example uses code from a post on [Stack Overflow](http://stackoverflow.com/questions/14492284/center-a-map-in-d3-given-a-geojson-object) to demonstrate how this problem can be solved a bit easier.  

In this example we'll load a coastline extract from OpenStreetMap of the New York City area. Then we'll scale and translate it using a bounding box and some math so that it fits well on the web page. 
