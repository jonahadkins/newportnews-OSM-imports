#Newport News, Virginia OSM Buildings Import

The City of Newport News GIS office graciously supplied shapefiles of building footprints and addresses upon request. 

###Pre-Processing 

* Building Footprints (82, 094 footprints, 53,558 addresses)  
  * Existing Building Classification Codes
    * 1 - Residential
    * 2 - Commercial
    * 3 - Public
    * 4 - Miscellaneous
    * 5 - Courtyards
    * 6 - Foundations  
  

* Resulting file was joined to address points layer and parsed address information was added to buildings file.  
* Calculated Building types over to OSM Tag methodology  
* Split building polygons by voting districts for manageable upload bits.  
* Existing OSM footprints were updated where applicable.  

Final building file attributes included:
* addr:housenumber
* addr:street (`prefix` + `name` + `type` + `suffix`)
* addr: city
* addr: state
* addr: postcode
* addr: unit  
* building: (= `yes` `industrial` `house`, etc)
* name
* amenity  


### Upload / Import To OSM  
Building footprint section were uploaded using JOSM with attributes mapped to the OSM Tag convention.  

#ToDo  

Import remaining secondary address points (33,477 Records)  
  

Yeah Open Data!

