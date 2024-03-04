# Natural-Disaster-Monitor

Background

The Natural Disaster Monitor (NDM) is an application that uses ArcGIS Maps SDK for JavaScript and Survey123. It allows for real time submission of disaster occurrences through user submitted forms. First responders, land managers, surveyors, scientists, engineers, and other environmental professionals will be able to catalogue disasters in real time. It has the functionality to log disasters, distinguish basic disaster categories (hydrological, meteorological, climatological, and geophysical), and the feature layer produced through this application can be used to perform spatial analysis to understand the freequency of disaster types, and to understand which areas are more prone to certain types of disasters. The categorization of disasters in the database follows a similar format to the EM-DAT (Emergency Events Database) and the Geocoded Disasters Dataset (GDIS). The EM-DAT is a database that catalogues every major natural disaster around the world, with basic information such as death toll, monetary damage, injury total, etc. The Geocoded Disasters Dataset (GDIS) is a subset of EM-DAT that adds location information about a disaster. 

How - To

The primary functionality of the application is to log disaster incidences. To do so, the user can click on the  "Report Disaster" link in the top right corner of the map. This link re-directs the user to a Survey123 form that was created using Survey123 Connect. The form allows the user to submit the following information about a disaster incident: 
  1. Date and Time Observed - Date and Time of disaster. Defaults to current time, but can be changed if reporting after the fact. Provide best estimates for time if unknown.
  2. Location - Location of disaster. Defaults to current location, but can be changed if reporting after the fact. Provide best estimates for location if unknown, or if disaster has multiple locations.
  3. Disaster Group - Meteorological disasters, Climatological disasters, Hydrological disasters, and Geophysical disasters.
  4. Disaster Type - Type of disaster. Populates depending on Disaster Group selection.
  5. Notes - Provide any additional information about the incident.

Once the form is filled out, a point will be added to the map in real time. This means that the feature layer has been updated, and information about the disaster has been added to the database hosted on ArcGIS Online. 

The secondary functionality of the application allows the user to click or tap on any point present on the map. This will display a pop-up containing all of the relevant information for that particular disaster. 

Note: A legend is not including in this version of the application because it is intended to be mobile first. The legend widget crowds the UI, and makes data hard to see on-screen. In future versions (desktop application etc), a legend will be added. Each feature contained in the map is labeled with identifying information so that any functionality that a legend provides is lost. 
