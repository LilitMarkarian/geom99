# Step by Step Logs

## Week 7 and 8 checklist 

### GCP - Creating and using provided image
1. Sign into GCP 
2. hamburger button 
3. Compute Engine 
4. VM Instances --> Enable 
5. "Create Instance" 
6. change the boot disk and add the Image provided --> Custom Images and change the project to the server that contains the image and click Select.. 
7. Enable Firewall to Allow HTTP and HTTPS traffic 8- Create!! 

### Set Up Firewall Rules
1. Create a Firewall Rule 
2. under the Direction of Traffic select Ingress and undet the Action on Match select Allow 
3. Under the Targets select All instances in the Network  
4. Source filter should be IPv4 ranges 
5. under the Source IPv4 ranges enter your External IP address ( should not start with 10.x.x.x or 192.168.x.x ) 
6. under Protocols and ports select TCP and enter ports 444, 6080, 6443  and click Create! this will create the Firewall rule!
   
Followed Shawn's video for the above steps 
**`https://www.youtube.com/watch?v=dyFeyBX9jIY`**

### To know your server is on and running you should look at the status of your instance on GCP.. 
If the instance is stopped the status will be set to ![image](https://github.com/LilitMarkarian/geom99/assets/97748633/46c223b1-60f9-4fe7-b869-9a3e4c380bc7)
and if the instance is running the status will look like ![image](https://github.com/LilitMarkarian/geom99/assets/97748633/3a691eed-5ca6-47eb-80db-e77920b1d96d)


### The recommended way to turn off the server is:
- To go to the three dots on GCP and stopping the VM --> ![image](https://github.com/LilitMarkarian/geom99/assets/97748633/b4e66023-6c7c-44f1-b656-44bc3b948957)
### To turn it back on, simply select the **Start/ Resume**

**Understand how these tools fit into the the Web, Middle and Data tiers discussed in class. The data tier can come many places, even a simple GeoJSON file. A web tier example is the ArcGIS Online web map, which provides the user experience wrapping the map service. The map service itself (from your ArcGIS Server on GCP) is the middle tier to power the web map with data, and ArcGIS Server connects (on the back end/not accessible over the web) to the database or data store. ** --> read these following articles to understand better 
`https://enterprise.arcgis.com/en/server/latest/publish-services/windows/services-in-arcgis-enterprise.htm`

`https://enterprise.arcgis.com/en/server/latest/publish-services/windows/relationships-between-web-services-and-portal-items.htm`

## Publishing an Image from the Server to ArcGIS Online
1. Open ArcGIS Pro
2. Go to Insert and Connections
3. ![Screenshot 2024-03-12 150822](https://github.com/LilitMarkarian/geom99/assets/97748633/9ac106f6-c537-4c92-89ec-d0a55e21f417)
4. ![Screenshot 2024-03-12 231650](https://github.com/LilitMarkarian/geom99/assets/97748633/e151d84f-808d-43fc-b0c3-3e78c8b3a3b8)
5. ![Screenshot 2024-03-12 150928](https://github.com/LilitMarkarian/geom99/assets/97748633/48887b6f-7468-4cd6-8b7e-a27b3a89fc05)
6. ![Screenshot 2024-03-12 144123](https://github.com/LilitMarkarian/geom99/assets/97748633/95c9b10e-d184-48bc-9e40-cb1306c70bc2)
7. Click on Share
8. Share As Web Map
9. Analyze/ Resolve all warnings or errors you encounter and then Click Share!
10. ![Screenshot 2024-03-12 150615](https://github.com/LilitMarkarian/geom99/assets/97748633/f22c7246-c933-411f-bd55-e9fbc49e7c46)

## Publishing a map service into ArcGIS Server on GCP VM
1. Open ArcGIS Pro
2. Go to Insert and Connections
3. ![Screenshot 2024-03-12 150822](https://github.com/LilitMarkarian/geom99/assets/97748633/9ac106f6-c537-4c92-89ec-d0a55e21f417)
4. ![Screenshot 2024-03-12 231650](https://github.com/LilitMarkarian/geom99/assets/97748633/ce8fb0c2-ffcc-429a-ab88-49849cc899be)
5. ![Screenshot 2024-03-12 231727](https://github.com/LilitMarkarian/geom99/assets/97748633/eca0efde-4d1e-4d63-8306-7e9555dbd208)
6. After clicking on Map Service from the previous image, it will open a folder to select your desired map.
7. This will open a Publish Map service tool. Fill out all the required information and fix all the errors and warnings.
8. One of the warnings is ![Screenshot 2024-03-12 230832](https://github.com/LilitMarkarian/geom99/assets/97748633/7f491d88-ebd7-458c-96ef-b948886dc544)
        To fix this you should register the folder, provide a connection details for the data source. Give it a name and the publisher folder should be your PC and the _Server folder Path_ should be set to **New Path** and paste C:\gisworkspace\Canada and Click **Create**!
9. After it registers the folder, if there are no more errors to solve --> Click **Publish**!! ![image](https://github.com/LilitMarkarian/geom99/assets/97748633/c18a4699-babf-4be4-8d6d-88471fe79523)
10. This will publish the map onto the Server ![image](https://github.com/LilitMarkarian/geom99/assets/97748633/3a373acf-227a-468a-b89b-14dfbdd9ce86)
      ![Screenshot 2024-03-12 231221](https://github.com/LilitMarkarian/geom99/assets/97748633/64bd601b-ccd6-45cc-9547-7fea5a1b71dd)





