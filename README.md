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
* Voyage ID (Automatically? generated unique ID for each voyage)
* Vehicle Type(Dropdown list: e.g. ship, helicopter, land vehicle)
* Vehicle Name/Identifier (e.g. Ship name, Rego number)
* Start Month (compulsory)
* End Month (compulsory)
* Start Date (if known)
* End Date (if known)
* Chief Scientist/Principle Contact Name
* Chief Scientist/Principle Contact Email
* Voyage description (free text field)
* Further information (Free text field)
* Berth availability (Y/N/U)
* Ocean Sector (drop down list of five SO regions. Select the region in which the majority of the cruise occurs.) 

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
