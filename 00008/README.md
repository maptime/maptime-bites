# D3JS: Translating and Transforming GeoJSON data
[D3JS](http://d3js.org/) is a JavaScript library for creating data-visualizations for the web using Scalable Vector Graphics (SVG). (For a quick primer on SVG see [this video](http://youtu.be/a2K_pOp2ydQ)). D3 features powerful [mapping funcitonalities](https://github.com/mbostock/d3/wiki/API-Reference#d3geo-geography) that let you create web-maps in all sorts of cartographic projections other than the [Web-Mercator](http://spatialreference.org/ref/sr-org/epsg3857-wgs84-web-mercator-auxiliary-sphere/). D3 also allows for interactivity and animation, both of which are not covered here but will be in a following tutorial. 

One of the problems of working with geospatial data a la cart in D3 is appropriately scaling and translating data. The goal is to demonstrate how this problem can be solved a bit easier than simple trial and error.

In this example we'll load a coastline extract from OpenStreetMap of the New York City metro area that has already been converted to a GeoJSON format and projected to a WGS84 coordinate reference system. We'll project this data to D3's Albers projection, then scale and translate it using a bounding box and some math so that it fits well on the web page. From here we can console.log the parameters of the scale and translation so that we can fine tune them a bit further.

The example in the index.html file within this repo uses code borrowwed from a post on [Stack Overflow](http://stackoverflow.com/questions/14492284/center-a-map-in-d3-given-a-geojson-object).
