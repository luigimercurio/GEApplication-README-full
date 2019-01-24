## Overview
Google Earth plugin for Commercial Real Estate professionals. Will present information about any property in
Miami-Dade County using a map-based interface

### Features
**Property mapping:** All properties are mapped according to their GeoLocation information (i.e. Latitude / Longitude)

**Color coding:** Properties are represented by colored pins, allowing the user to distinguish between condos /
cooperatives and single-owner properties

**Active information access:** Information is accesible py *"pushing"* a pin identifying the property and opens an
*"information bubble"* within the Goggle Earth screen

**Layered information access for condos/cooperatives:** When a condo/coop pin is pushed, a list of all individual
parcels present in the condo/coop is presented, allowing easy access to each one of them

**Multiple information sections:** Several clearly separated sections are present on the information bubbles:
- General property information (address, folio number, ownership, land use, square footage, floors, units, etc.)
- Parcel contour (on aerial map)
- Tax assessment information
- Value assessment information (comparative through last 3 years)
- Tax benefits information (if applicable)
- Full legal description
- Sale history
- Zoning information (with municipal zoning code)
- Individual building information for multi-building properties
- Extra features (pools, sprinklers, patios, elevators)
- Land use and governmental restrictions

**Google Earth integrated features:** The application takes advantage of ready available GE features:
- Available both on desktop and mobile
- Current position mapping
- Street maps and aerial maps
- Street views

### Technologies
- Google Earth (main content delivery application)
- HTML (for description bubbles)
- CSS (for bubble styling)
- KML/XML (for pin positioning)
- SQL (MySQL server for data storage)
- HTTP (delivery protocol for KML and HTML)
- Apache Tomcat (Server is a web application hosted in a Tomcat container)
- CSV (County data is delivered in CSV format and has to be parsed and inserted in the SQL database)
- Java (Main language used on the web server)
- Javascript (Templating language on the web server)
- Spring / Spring Boot (Server is developed as a Spring Boot application)
- KML/XML/HTML templating (this is implemented through self-developed Javascript View Resolver)

### What I'll Have to Learn
- KML positioning of pins within Goggle Earth
- Dynamic reloading of pins upon map navigation
- Embedding HTML within KML descriptors
- Translating CSV tables into SQL tables
- Implementing GeoLocation search on database
- Integrate Spring / Spring Boot with Tomcat containers
- Logging within Tomcat container environment