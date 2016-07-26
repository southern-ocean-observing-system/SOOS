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
|Voyage ID|Yes|Free Text|Automatically generated unique ID for each voyage)|
|Vehicle Type|Yes|Dropdown list|e.g. ship, helicopter, airplane, land vehicle, convoy,other|
|Vehicle Name/Identifier|Yes|Free Text|e.g. Ship name, Rego number|
|Start Month|Yes|YYYY-MM||
|End Month|Yes|YYY-MM||
|Start Date|No|YYYY-MM-DD||
|End Date|No|YYYY-MM-DD||
|Chief Scientist/Voyage Leader Name|Yes|Free Text|80 chars|
|Chief Scientist/Voyage Leader Email|Yes|Free Text|80 chars|
|Voyage description|Yes|Free Text| 1000 chars|
|Further information|No| Free Text|1000 chars|
|Berth availability|Yes|Dropdown menu - Y/N/U||
|Ocean Sector|Yes| Dropdown menu, illustrated by a map of SOOS regions|Indian Sector, Weddell/Dronning Maud Land, West Antarctic Peninsula, Amundsen/Bellingshausen Sector, Ross Sector| 

## Fields for individual projects 
* Voyage ID (From the cruise transect table)
* Project ID (Assigned by PI)
* Project Name
* Principle Investigator name
* Principle Investigator email
* Project Description
* URL for further information
* Essential Ocean Variable being studied (drop-down list - ability to pick multiple options)
* Funding status

## Spatial Information

* Layer of common ports
* Add lines, polygons, points for cruises
