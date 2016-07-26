# SOOS
Southern Ocean Observing System data projects


## Wish list

- shiny form for user input
- linked map for voyage plan via GeoJSON
- submit / edit for plan
- select / view by project search, geographic bound, date range, search by data type etc. 
- Make it pretty

## Promising leads

- Shiny as overarching system for web pages and publishing (Explore gallery for examples with maps you can draw in)
- explore leaflet and mapview packages in R for drawing tracks
- use dplyr and RSQLite as the data base backend
- use DT to present (and edit?) tabular data within Shiny

## Fields for cruise transects
|**Field Name**|**Compulsory?**|**Data Type**|**Notes**|
|--------------|---------------|-------------|---------|
|Voyage ID|Yes|Free Text|20 chars, self-assigned unique ID|
|Vehicle Type|Yes|Dropdown list|e.g. ship, helicopter, airplane, land vehicle, convoy,other|
|Vehicle Name/Identifier|Yes|Free Text|100 chars, e.g. Ship name, Rego number|
|Start Month|Yes|YYYY-MM||
|End Month|Yes|YYY-MM||
|Start Date|No|YYYY-MM-DD||
|End Date|No|YYYY-MM-DD||
|Chief Scientist/Voyage Leader Name|Yes|Free Text|50 chars|
|Chief Scientist/Voyage Leader Email|Yes|Free Text|50 chars|
|Voyage description|Yes|Free Text| 1000 chars|
|Further information|No| Free Text|1000 chars|
|Berth availability|Yes|Dropdown menu - Y/N/U||
|Ocean Sector|Yes| Dropdown menu, illustrated by a map of SOOS regions|Indian Sector, Weddell/Dronning Maud Land, West Antarctic Peninsula, Amundsen/Bellingshausen Sector, Ross Sector| 

## Fields for individual projects
|**Field Name**|**Compulsory?**|**Data Type**|**Notes**|
|--------------|---------------|-------------|---------|
|Voyage ID|Yes|Automatic??| From the cruise transect table|
|Project ID|Yes|Automatic| Unique Project ID|
|Project Name|Yes|Free Text||
|Principle Investigator Name|Yes|Free Text|50 chars|
|Principle Investigator Email|Yes|Free Text|50 chars|
|Project Description|Yes|Free Text| 1000 chars|
|URL for further information|Yes|Free Text|200 chars|
|Essential Ocean Variables being studied|Yes|Drop-down menu with ability to pick multiple options|(Pip to generate list)|
|Funding status|Yes| Dropdown menu|e.g. Funded, Not yet funded|

## Spatial Information

* Layer of common ports
* Add lines, polygons, points for cruises
