# Inside Airbnb

- ## Purpose:
  Experimentation with data sets in IBM Cognos\
  I wanted to compare data from different cities in different countries...see what options are per city
  
  ### Quarterly data for the last year for each region used:

    Boston, Massachusetts, United States as of 19 March, 2023

    Copenhagen, Hovedstaden, Denmark as of 31 March, 2023

    Dublin, Leinster, Ireland as of 15 March, 2023

    Edinburgh, Scotland, United Kingdom as of 17 March, 2023

    London, England, United Kingdom as of 14 March, 2023

- ## Process:
  Downloaded desired cities data set as a CSV file from open data source, uploaded listings.csv into google sheets (my excel is out of date), minimally cleaned data to desired metrics, created pivot tables to create one condensed excel sheet as an overview of all 5 cities desired metrics

  The Cognos dashboards focused on individual cities- number of listings [Key performance indicators (KPIs), formatted and rounded], average price [Key performance indicators (KPIs), formatted and rounded], what kind of lodging accommodations available (tree map or pie chart), and locations (map). Instead of doing the same exact format for every single city, I wanted to experiment with minor variations from color and layout to different visualizations for the same information.

  ### Boston, Massachusetts, United States
  Number of listings: 3.86K (KPI average calculation)\
  Average Price: $190.61 (KPI average calculation)\
  Lodgings Available: tree map\
  Listing locations: map (longitude and latitude used, street view, labels when hooving on individual locations include neighborhood, price, and room type)

  ### Copenhagen, Hovedstaden, Denmark
  Number of listings: 14.8K (KPI average calculation)\
  Average Price: $1,407 (KPI average calculation)\
  Lodgings Available: pie chart comparing percentages of lodging as a whole\
  Listing locations: map (longitude and latitude used, street view, labels when hooving on individual locations include neighborhood, price, and room type, as well as added a heat-cluster layer)
  
  ### Dublin, Leinster, Ireland
  Number of listings: 7.88K (KPI average calculation)\
  Average Price: $207.92 (KPI average calculation)\
  Lodgings Available: pie chart comparing percentages of lodging as a whole & word cloud\
  Listing locations: map (longitude and latitude used, satellite street view, labels when hooving on individual locations include neighborhood, price, and room type, as well as added heat map with neighborhood regions layer)

  ### Edinburgh, Scotland, United Kingdom
  Number of listings: 7.25K (KPI average calculation)\
  Average Price: $160.33 (KPI average calculation)\
  Lodgings Available: tree map & word cloud\
  Listing locations: map (longitude and latitude used, street view, labels when hooving on individual locations include neighborhood, price, and room type)

  ### London, England, United Kingdom
  Number of listings: 75.2K (KPI average calculation) & image depiction\
  Average Price: $175.73 (KPI average calculation) & image depiction\
  Lodgings Available: tree map\
  Listing locations: map (longitude and latitude used, view is inherited from theme, labels when hooving on individual locations include neighborhood, price, and room type, as well as added a heat layer and neighborhood regions layer with labels)

  ### Overview of All 5 Cities
  Experimented with transparency, filters, graphs
  Unfortunately, came across limitations with colors and fonts as well as dodgy responsive designs (the values present do not necessarily show up in edit mode)


  
- ## Learned/Issues & Problems:
  Some of the metrics used in the CSV files are unknown i.e. price- is it in U.S. dollars?, is it daily price?\
  Cognos formatting issues when exporting dashboard into PDF\
  The little intricacies of each of the dashboards cannot fully be appreciated by PDFs and screenshots\
  Limitations with formatting and layouts in Cognos\
  Learned the visualizations and styles that I am particularly fond of and the desire to keep experimenting\
  Importance in information being legable and not too busy



## Credit

All data info was retrieved from:

Inside Airbnb
Adding data to the debate

http://insideairbnb.com/get-the-data/

The site uses the following Open Source technologies:- D3, Bootstrap, Python, PostgreSQL and Google Fonts.
Maps are designed in Mapbox with OpenStreetMap data and hosted via Mapbox.
The site is served by an Amazon S3 "bucket".

Files available:

| Country/City | File Name | Description |
| ----------- | ----------- | -------- | 
|     	     | listings.csv.gz	|         Detailed Listings data |
|     	     | calendar.csv.gz	|         Detailed Calendar Data |
|     	     | reviews.csv.gz	|         Detailed Review Data |
|     	     | listings.csv	|         Summary information and metrics for listings in Boston (good for visualisations). |
|     	     | reviews.csv	|         Summary review data and Listing ID (to facilitate time based analytics and visualisations linked to a listing). |
|     	     | neighbourhoods.csv |    Neighbourhood list for geo filter. Sourced from city or open source GIS files. |
|     	     | neighbourhoods.geojson	|    GeoJSON file of neighbourhoods of the city. |

_____________________________________



