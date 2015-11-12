{
   "categories": [],
   "date": "2015-10-27T15:57:52-07:00",
   "description": "",
   "draft": false,
   "slug": "",
   "tags": [
      "map",
      "leaflet"
   ],
   "title": "zero",
   "type": "leaflet"
}

# Demo Zero, copied from leaflet-map QuickStart Guide in README.md

  * [leaflet-map on Github](https://github.com/leaflet-extras/leaflet-map/)
  * [view source](view-source:http://stephen-marshall-moore.github.io/demo/map_zero)
  * using [branch (leaflet 1.1.0)(https://github.com/leaflet-extras/leaflet-map.git)
    - resulting error (in Chrome Version 45.0.2454.99 (64-bit) on openSuse Tumbleweed)
      * Error: Invalid value for <path> attribute d="M0,-7.649338877763425e+302A7.649338877763425e+302,7.649338877763425e+302,0,1,1,-0.1,-7.649338877763425e+302 z"
      * from what I dug through this is the result of the SVG intrepeter in Chrome only accepting single precision floats and this contains double precision representations what I haven't dug into is where the large numbers arise from
      * If the leaflet-circle is removed then the error does not occur but no tiles is displayed
      * Moving the circle from the same location also removes the error (no tiles displayed, beyond zoom?)
  * using [branch use_bounds_for_fit_to_markers](https://github.com/stephen-marshall-moore/leaflet-map/tree/use_bounds_for_fit_to_markers)
    - [resulting map](/demo/map_zero)
 

