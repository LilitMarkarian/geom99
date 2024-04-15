# My solution for the final exam Part 1 Question
### The Following are the criteria and resources for the problem
`Currently some individuals in the local government use QGIS as GIS desktop software, but are no experts. They are open to switch to commercial software if they can have it funded by this solution.` 
As some people already know how to use QGIS as GIS Desktop software, I did not want to change what they already know.

`The local government has no server infrastructure and no capacity to host web sites or servers. Their IT department is minimal and only supports windows desktop machines.`
Instead of creating new server infrastructure as their IT department is minimal and only supports windows desktop machiens, I decided to go with QGIS Cloud Pro.
- It is a paid solution which is $95 CAD per month --> 1140/Year for 500gb. extra 1gb per month could be added if needed for an extra $30cad per month. Which comes to $1500cad/year.
- The owner could decide who can access the data/map. However, the user should have access to QGIS Cloud (Not Pro) which is free of cost. 
- Some of the features include:
   - WebGIS Client on / off
   - Mobile Client on / off
   - WMS access password protected
   - WebGIS Client password protected
   - Search types : OpenStreetMap search, GeoNames search, customizable database search
   - Fixed scales
   - Customizable WebGIS Client
   - Number of databases: 10 (Additional databases for 60 €/month per 10 databases)
   - User administration
   - Editing in WebGIS client
   - Available space for data : 500mb (could buy more (1gb for $30cad/month)
   - SSL support
   - Custom domain names (map.mycompany.com)
   - Editing Through Web Feature Services
   - Viewer personalization (logo, colors, etc)
- QGIS Cloud Pro could also be connected to PostgreSQL and PgAdmin3

`The real estate agents need to see parcel ownership boundaries (4,000 parcels polygon records) over some type of aerial image.`
OpenStreet map or Leaflet basemaps could be used as a baselayer and the 4000 parcels polygons on top. Those could be created using the QGIS Desktop version and then import to the Cloud to then use it for the webmap. 

`The parcels data from the province are available as a GeoPackage download or as an ArcGIS Server Map Service, your choice. The solution must be updated at least each week with a fresh parcel layer (if necessary).`
The layers that need to be updated could be updated using QGIS Desktop and by using the Cloud pluggin we could publish it to the QGIS Cloud Pro. (very similar to Esri)

`The city also has data for roads (2,200-line segments), parks (23 polygons), address points (5,500 points), which are updated a no more than 6 times per year and would be ideal to show those on the map as well.`
These could be used as basemaps (not operational layers) and updating them is the same process as the previous step. 

`If there are any ongoing (monthly/yearly) costs for the proposed solution, Real Estate Agents will need to pay a fee for access to the proposed system. This can recover ongoing monthly costs incurred by the local government. If any monthly costs exists there must be a way to create accounts (security) for each agent to log in on the system to manage access. An estimate of costs is fine, exact figures are not necessary.`
As the Real Estate Agents right now are paying $60 per printed map, instead of paying for the map as it will be on the web, they could pay for the Cloud and storage which would come cheaper than paying $60 for one print. 

# web 
-  Using The **QGIS2Web** plugin we could create interactive web maps directly from **QGIS** Deskop without any coding. However, to use it in the **Cloud** we should look for **QGIS Cloud plugin**

It is worth mentioning that QGIS also works with Python Scripts to automate any tasks. (PyQGIS)

### Sources: 
> QGIS Cloud Pro price and features info: https://qgiscloud.com/pages/plans?locale=en

> How ot add users to the access list: https://support.qgiscloud.com/kb/faq.php?id=6#:~:text=Choose%20your%20map%20and%20click%20on%20the%20pen-icon,only%20available%20with%20a%20QGIS%20Cloud%20Pro%20account

> QGIS Projects into Interactive Online Maps: https://mapscaping.com/qgis-projects-into-interactive-online-maps/#:~:text=In%20this%20blog%20post%2C%20we%E2%80%99ll%20walk%20you%20through,data%20and%20visualizations%20with%20a%20wider%20audience%20online

> Free web maps: https://gisgeography.com/qgis-cloud/#:~:text=You%20can%20publish%20your%20maps%20free%20of%20charge,Pro%20is%20the%20only%20way%20to%20do%20that

> In Details: https://docs.qgiscloud.com/en/

> Running and Scheduling QGIS Processing Jobs: https://www.qgistutorials.com/en/docs/running_qgis_jobs.html
