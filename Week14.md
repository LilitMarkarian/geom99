# Week14
## Task Scheduler AGOL Jupyter Notebook
This tool was very easy to use once you find where it is. 
- Open AGOL and go to your Jupyter Notebook.
- After writing your code if you're happy with it and want to automatically run in every week, you could create a task scheduler.
- Task Scheduler will run your code however you configure it. In the following example I configured it so it runs every week on Monday at 6am.
    ![CreateTask01](https://github.com/LilitMarkarian/geom99/assets/97748633/e68cc639-64f2-48c6-bac5-812096891183)
    ![CreateTask02](https://github.com/LilitMarkarian/geom99/assets/97748633/2ff70fe9-aafa-4abc-8445-7750f575975d)
- Once it's configured, it is ready to go. There is nothing else to do other than wait for next Monday 6am.
- Well... That is not what I did. I configured another task for only 15 minutes just to test if it is working. And after checking it after 40 minutes, it already generated 3 reports (as my code was generating reports)
     ![CreateTask03](https://github.com/LilitMarkarian/geom99/assets/97748633/b4016ecf-dcdc-42d0-b9d9-bd80c0da48b1)
and these are the generated reports in AGOL. ![image](https://github.com/LilitMarkarian/geom99/assets/97748633/7c6cf70c-2dce-425b-8751-4d1a886591b4)
- Also, if you wish to pause/edit/delete the scheduled task you could simply the three dots next to your task and choose the option you want to use.
     ![Screenshot 2024-04-10 112448](https://github.com/LilitMarkarian/geom99/assets/97748633/badad385-d7ba-4d3e-84cd-84a6daacf596)
 
> I liked working with Jupyter Notebook and found it interesting to see how it could automatically run the code however you configure it.

## Windows Task Scheduler System
> There are things to learn about this system to be able to do this. However, I just wanted to test it (and it did not work).
- Create a new Task and fill our the General task ![Screenshot 2024-04-10 234014](https://github.com/LilitMarkarian/geom99/assets/97748633/d9e4fbea-b77b-40f6-b32c-c96306924359)
- Go to Trigger and create a New Trigger. Configure the New Trigger however you wish.. ![Screenshot 2024-04-10 234340](https://github.com/LilitMarkarian/geom99/assets/97748633/17c607b6-5327-4d63-a368-57a18ce43f66)
- Now go to Actions. Create a New action and choose if you want the Action to be **Starting a program, Sending an E-mail(Deprecated), or display a message(Deprecated)**. for my example, I chose Send an E-mail. ![image](https://github.com/LilitMarkarian/geom99/assets/97748633/e3530a91-071d-4c51-bc34-674d394160de)
- After Googling and trying a few options for the **SMTP Sever:** I was still unable to make it work. I will keep working on this and hopefully be able to successfully run it as it would help so much for our project.

## Website
Other than those two task schedulers I worked on our website this week. 
