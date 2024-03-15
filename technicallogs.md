# Step by Step Logs

# Week 7 and 8  

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
4. ![Screenshot 2024-03-12 150900](https://github.com/LilitMarkarian/geom99/assets/97748633/04023a1b-74ba-42ba-b10b-f5c1e976f1b6)
5. ![Screenshot 2024-03-12 150928](https://github.com/LilitMarkarian/geom99/assets/97748633/b70a19e2-9dde-4192-a289-992ebbfacb3c)
6. ![Screenshot 2024-03-12 144123](https://github.com/LilitMarkarian/geom99/assets/97748633/95c9b10e-d184-48bc-9e40-cb1306c70bc2)
7. Click on Share
8. Share As Web Map
9. Analyze/ Resolve all warnings or errors you encounter and then Click Share!
10. ![Screenshot 2024-03-12 150615](https://github.com/LilitMarkarian/geom99/assets/97748633/f22c7246-c933-411f-bd55-e9fbc49e7c46)

## Publishing a map service into ArcGIS Server on GCP VM
1. Open ArcGIS Pro
2. Go to Insert and Connections
3. ![Screenshot 2024-03-12 150822](https://github.com/LilitMarkarian/geom99/assets/97748633/9ac106f6-c537-4c92-89ec-d0a55e21f417)
4. ![Screenshot 2024-03-12 231650](https://github.com/LilitMarkarian/geom99/assets/97748633/e151d84f-808d-43fc-b0c3-3e78c8b3a3b8)
5. ![Screenshot 2024-03-12 231727](https://github.com/LilitMarkarian/geom99/assets/97748633/55da5606-8e95-4d4e-9fb3-9cb257b90629)
6. After clicking on Map Service from the previous image, it will open a folder to select your desired map.
7. This will open a Publish Map service tool. Fill out all the required information and fix all the errors and warnings.
8. One of the warnings is ![Screenshot 2024-03-12 230832](https://github.com/LilitMarkarian/geom99/assets/97748633/7f491d88-ebd7-458c-96ef-b948886dc544)
        To fix this you should register the folder, provide a connection details for the data source. Give it a name and the publisher folder should be your PC and the _Server folder Path_ should be set to **New Path** and paste C:\gisworkspace\Canada and Click **Create**!
9. After it registers the folder, if there are no more errors to solve --> Click **Publish**!! ![image](https://github.com/LilitMarkarian/geom99/assets/97748633/c18a4699-babf-4be4-8d6d-88471fe79523)
10. This will publish the map onto the Server ![Screenshot 2024-03-12 231215](https://github.com/LilitMarkarian/geom99/assets/97748633/1ff812ce-d4bf-4975-bd85-64770de1c8f8)

    ![Screenshot 2024-03-12 231221](https://github.com/LilitMarkarian/geom99/assets/97748633/7a59fcc1-3b69-49b2-8ac7-654e9dcc264d)

# Week 9 
## ArcGIS WorkForce
- Open AGOL
- Next to your name there's ![image](https://github.com/LilitMarkarian/geom99/assets/97748633/4decabc6-cbbf-4d77-8952-e411d9d4df46) Click on it and find ![image](https://github.com/LilitMarkarian/geom99/assets/97748633/e04ab408-49fe-42eb-99d2-36cdef3cad7d)
- You could see ![image](https://github.com/LilitMarkarian/geom99/assets/97748633/26283d63-1bb7-4db7-a77f-6cc93fe2e0a7) Click on it and Name your project and Create Project.
- Add Assignment types (As many as you want) and add workers to the assignemnt. (I assigned myself for testing)
     - ![image](https://github.com/LilitMarkarian/geom99/assets/97748633/edaea52d-e546-4614-9f62-5f30d30894b3)
     - ![image](https://github.com/LilitMarkarian/geom99/assets/97748633/ac132452-c6dd-480e-940f-3bcaf131eb84)
- After adding the assignment type and workers we could start working on the map

### ArcGIS WorkForce Map
-  We could create assignments by clicking on ![image](https://github.com/LilitMarkarian/geom99/assets/97748633/dd16f0bd-2320-4874-affb-3e6003260139)
- Creating an Assignment and assigning it to a worker is very easy (The Blue pin is the new assignment location)
  ![image](https://github.com/LilitMarkarian/geom99/assets/97748633/3b500527-4731-4ad6-b769-a3d63686856d) 
- WorkForce has a mobile application. The assigned person (if the notifications are on for the app) would get a notification that they have been assignemd for an assignment.
   ![image](https://github.com/LilitMarkarian/geom99/assets/97748633/7d9551e1-b61f-48ef-ba07-ab12e420406b)
- Clicking on the notification -- or opening the WorkForce Application would show them the Assignment that they have been assigned to.
 ![MicrosoftTeams-image (17)](https://github.com/LilitMarkarian/geom99/assets/97748633/00ef18a2-5e9a-4a51-b1ef-6415efd49f4a)
- The person assigned to a job could Accept the job or Decline it. 
![MicrosoftTeams-image (13)](https://github.com/LilitMarkarian/geom99/assets/97748633/bc4ad429-6b0e-48c3-98d9-bc75d2d8b1ca)
- The application also has the option to use Google maps or phone maps to show the directions to the assignment area which I found very interesting.

### WorkForce WebApp
- The manager can track on the WebApp if the job was completed or not by going to the project and checking the Status.
  ![image](https://github.com/LilitMarkarian/geom99/assets/97748633/bcfa930d-2896-48c1-8415-b8f81cf29b6f)
- They could also filter the status type they wish to see by going to ![image](https://github.com/LilitMarkarian/geom99/assets/97748633/3a2a7c13-68cc-4b41-b151-77c1a18379e7) and ![image](https://github.com/LilitMarkarian/geom99/assets/97748633/2680a6e1-0bd3-4bbb-8561-baf4ac92c5e1) choosing one of these status options. 

### WorkForce Data on AGOL
- To see the data we could simply go to the layer and open its data.
- Doing so would show us when the assignment was completed, who completed the assignemnt, and if there are any notes that the person added.
 ![image](https://github.com/LilitMarkarian/geom99/assets/97748633/14ef4be3-342b-4055-81f6-866f65744cd0)
- The layer could also be seen using Map Viewer or Map Viewer Classic.

## ArcGIS Solutions (conservation Easement Monitoring)
- In AGOL Find the Solutions Application ![image](https://github.com/LilitMarkarian/geom99/assets/97748633/460dfcfb-584f-4e4b-98cc-efb563592134)
- Find a Solution that works best with your project
- and Deploy it.
`How to deploy a solution --> https://doc.arcgis.com/en/arcgis-solutions/latest/get-started/deploy-an-arcgis-solution.htm#GUID-CB97DDF0-613C-4FA1-B8AC-BA0A2CBF671D`

### More about the Solution `https://doc.arcgis.com/en/arcgis-solutions/latest/reference/introduction-to-conservation-easement-monitoring.htm`
- I tested and played with multiple solutions -- Sign management, Conservation Easement Monitoring, and Citizen Problem Reporter. However, after looking into the Sign Management and testing it I realized it was not the best solution for our project and started looking more into the Conservation Easement Monitoring.
- This solution requires ArcGIS Online, ArcGIS Field Maps, ArcGIS Survery123, and ArcGIS COnnect.
  
### Configuring and testing the solution 
- After deploying the Solution on your account, it would show its content on your AGOL as well as when you go to the Solutions page it will be under _My Solutions_ ![image](https://github.com/LilitMarkarian/geom99/assets/97748633/f05fe459-8ca5-4bbe-a7db-48e0602238ba)
- The deployed Solution has ![image](https://github.com/LilitMarkarian/geom99/assets/97748633/caa7b8da-f8c9-42f7-abea-44b445d43046).
- I created Observation Points ad Conservation Easements area ![image](https://github.com/LilitMarkarian/geom99/assets/97748633/3ac94e8b-3369-40d6-83a9-5867af6a673e) using Map Viewer on AGOL.
- The same map could be used for data collection using Mobile FieldMaps Application -->  ![MicrosoftTeams-image (10)](https://github.com/LilitMarkarian/geom99/assets/97748633/99f30cb7-66eb-45e9-a5fc-dfa40d5c0745)
- This solution also has Dashboards with it which could be modified and edited as the user wishes ![image](https://github.com/LilitMarkarian/geom99/assets/97748633/ed2dadc8-bf7f-4072-bd4d-12ec29264c74)

> Despite the fact that I enjoed deploying this solution and understanding it, I do not think it is a great solution for our client. Comparing this solution with WorkForce, I believe workforce is a better solution for the project.

## Field Maps 
- ![image](https://github.com/LilitMarkarian/geom99/assets/97748633/7f1f09d4-59a9-4f2c-9894-bc871bbd249b) Created a new project in Field maps and started from 0.
- Doing so I was able to create a new table with felds I configured. ![image](https://github.com/LilitMarkarian/geom99/assets/97748633/a9aca455-3aff-4bcb-a8fe-831c86cf9de6)
- It is very easy to create and configure Field Maps.

### Creating an Offline Map
- Field Maps support Offline mapping as it takes into consideration areas that have little to no internet connection services.
- Creating Offline maps helps the user to collect data on the field while having no internet connections, and then when connected they could sync the map so that it would show on AGOL.
    - ![image](https://github.com/LilitMarkarian/geom99/assets/97748633/68d88d0a-f0e9-43cb-86f6-d4a3a0f239b6)
    - ![image](https://github.com/LilitMarkarian/geom99/assets/97748633/07d64cfd-b0a5-4806-b4b5-35c3bc2287dc)
    - On the mobile app it shows the online maps and the offline ones. ![MicrosoftTeams-image (9)](https://github.com/LilitMarkarian/geom99/assets/97748633/879dd2d5-d7de-4dd4-891e-ce64442a3da5)
    - choosing the offline map will only open the map that is in the red square. This helps with fast data load ![MicrosoftTeams-image (6)](https://github.com/LilitMarkarian/geom99/assets/97748633/ec3b0544-8d49-43a4-b1fd-1b1b12c710ca)

> Working with real data is more exciting and motivating, having to create fake data to test these solutions is not as satisfying. However, playing with these products thought me Very much about how each one of them work and it let me understand better what is needed for our project.

# Week 10 
















