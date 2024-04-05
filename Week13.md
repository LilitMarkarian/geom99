# Week 13
## Jupyter Notebook AGOL
To use Jupyter Notebook:
- Go to ArcGIS Online
- On the navbar click on _Notebook_ ![image](https://github.com/LilitMarkarian/geom99/assets/97748633/c500367a-78c4-4e49-9f98-f6d16c76e5f1)
- If you do not have a notebook yet, click on New Notebook_ ![image](https://github.com/LilitMarkarian/geom99/assets/97748633/28a450d5-f43b-4739-9080-9d92bd5dca35)
- Depending on the work you are doing, choose one of these options ![image](https://github.com/LilitMarkarian/geom99/assets/97748633/6ff497fc-1a2b-457f-a321-9e760fa2a187)
  - For our project I chose the Standard one.

### Sources 
`I used multiple sources on youtube, ArcGIS API for Python, and github to learn and test.` 
`Sources:
- https://www.youtube.com/watch?v=fCvs310AlhY
- https://www.youtube.com/watch?v=dzAbLFVuWiw
- https://developers.arcgis.com/python/api-reference/arcgis.apps.survey123.html
- https://developers.arcgis.com/python/samples/find-top-n-items-in-your-org/
- https://github.com/nzjs/Automated-Survey123-Reports (looked at this but have not used)`

## Report generation using ArcGIS API for Python - Jupyter Notebook.
- For this project I wanted to connect jupyter notebook to a Survey123 data to be able to generate reports. However, because I was not the owner of the survey123, I was not able to generate a report or create a template for it.
- After spending hours on this step, I decided to explore another way of seeing the data and understanding how jupyter Notebook works.
- I started exploring the feature layer that takes the data from the survey123 I was using before.
    - ![image](https://github.com/LilitMarkarian/geom99/assets/97748633/c97bc668-659d-4924-9c3c-e7222878b2ff)
    - ![image](https://github.com/LilitMarkarian/geom99/assets/97748633/0540e8b9-b2e8-4f62-9166-0b72049ff145)
    - ![image](https://github.com/LilitMarkarian/geom99/assets/97748633/2f5d4556-81de-4f19-a78a-ce90ce1b9179)
- After seeing the results of these codes, I was motivated to export it as a report .csv file. ![image](https://github.com/LilitMarkarian/geom99/assets/97748633/d11003ad-d0b7-45e5-91d0-1a9b46baed3b)
- This did not generate any reports into my folder so I decided to create my own survey123.

### Source:
`https://github.com/Esri/Survey123-tools/blob/73cee0b6f6c94edfc08b4037c27f96b79d2ff226/Work_with_Survey_Data/work_with_survey_data.ipynb`

## Generating Reports Using ArcGIS Online Survey123 - Jupyter Notebook
> The main goal of this task was to generate a report of survey123 data and download it locally using Jupyter Notebook.
> To make this work, we need to create a **report template** from our **_Survey123 website_**. 
- Open ArcGIS Online
- Because I created a _Solution_ that contained a survey123 in it (Parks and Grounds), I did not need to create a new one. However, for this to work You must be the owner of the survey.
- Go to the Survey123 item on AGOL
- Click _Open in Survey123_ and choose _Manage in Survey123 Website_ ![image](https://github.com/LilitMarkarian/geom99/assets/97748633/ecaa800c-8120-4eda-b060-345949b893d6)
- go to ![image](https://github.com/LilitMarkarian/geom99/assets/97748633/99c56eca-aa73-435e-b7a3-0f7100ffbc8d) from the navbar.
- And Click on Report ![Screenshot 2024-04-05 004158](https://github.com/LilitMarkarian/geom99/assets/97748633/354a4895-4eca-4ae9-98bf-6c90dc1878fc)
- Click Manage Templates ![Screenshot 2024-04-05 004431](https://github.com/LilitMarkarian/geom99/assets/97748633/bd65b001-3707-4a37-8f44-961a6ba3edff)
- 


