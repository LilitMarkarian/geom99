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


