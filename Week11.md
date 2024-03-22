# Week 11
- [x] Gathered data to start creating FieldMap training Content.
- [x] Created an _Microsoft Power Automate_ Email. It gets triggered when a new feature is created on Field Maps.

## Gathered Data to Start Creating Field map training Content.
In the training content I will be showing Fire Hydrants in Montreal parks. I used open sources to download the data and manipulated the spatial data using ArcGIS Pro. I will be working more on this next week as I will have the data ready and only record the videos.

## Microsoft Power Automate 
Because our customer is interested in automated repopr

### Step by step 
1. Sign in, Click on Connections, and then New Connection. ![Screenshot 2024-03-21 214443](https://github.com/LilitMarkarian/geom99/assets/97748633/fdc1a1fb-38eb-42f8-abe7-84746c98b7f2)
2. Search for **ArcGIS**![Screenshot 2024-03-21 214731](https://github.com/LilitMarkarian/geom99/assets/97748633/1a46309d-4514-4b80-ac48-76af296a9a58)
3. Click **_Create_**
4. After Clicking Create it will bring you to ![Screenshot 2024-03-21 214753](https://github.com/LilitMarkarian/geom99/assets/97748633/fe4bfb6b-d0fd-4543-b2e8-39a43d2db300) click Allow to let Pwer Automate access ArcGIS Online.
5. Go to **My Flows** and Click **New Flow** ![Screenshot 2024-03-21 214840](https://github.com/LilitMarkarian/geom99/assets/97748633/b2b456c1-eb54-4ec3-b28a-de6012e192e7)
6. Add _Flow Name_ and _Choose your Flow's Trigger_ ![Screenshot 2024-03-21 215658](https://github.com/LilitMarkarian/geom99/assets/97748633/23e8b9ff-a39d-4f71-8eee-fade12c4e551)
   - When choosing the Flow's Trigger, in the search bar search for ArcGIS to only see the triggers available for ArcGIS.
   - And Click **Create**
7. Under Parameters choose your feature layer (these are maps that you created or ones that are shared with you) ![Screenshot 2024-03-21 215902](https://github.com/LilitMarkarian/geom99/assets/97748633/76172f71-026d-44ee-9409-09ce3e65a34f)
8. After choosing the Feature to use, Click the Plus sign and add an action. In the search bar write "send an email" and choose the best option for you.
    ![Screenshot 2024-03-21 220019](https://github.com/LilitMarkarian/geom99/assets/97748633/d5da7e15-93a3-4395-b24e-a6617aaaea18)
10. You could set it to send to as many people as you wish. Add a subject and a text (these will not be changed unless you change them). You could also add Importance to these automated emails which could be set to either Normal, Low, or High. ![Screenshot 2024-03-21 220727](https://github.com/LilitMarkarian/geom99/assets/97748633/a5877c3f-7cb6-4558-9d63-bb42d22b988f)
11. I was very excited to save/run this tool and test it. However, unfortunately I got this Warning --> ![Screenshot 2024-03-21 220913](https://github.com/LilitMarkarian/geom99/assets/97748633/b85027b1-8aa7-4e6f-b5c1-8ffcca30c722).
12. I will keep looking into this product as I believe it is a powerful tool for our project.





