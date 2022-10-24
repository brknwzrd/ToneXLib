# ToneXLib

You will need to make sure you have updated to the latest ToneX version and opened it at least once before starting this proces.

These are CSV files which you can import into your ToneX library.db using an SQL editor like SQLiteBrowser.

The first thing you will need is SQLite Browser which you can get here for free https://sqlitebrowser.org/

Next you need the CSV files which are essentially just a list of the models that have been uploaded to ToneNet. Each CSV file contains models uploaded between the dates indicated in the file name, this is due to upload file size limits on github. You will need to repeat the process for each CSV to get the maximum number of models.

Once you have SQLite installed you'll want to open your Library.db

![image](https://user-images.githubusercontent.com/116271180/197430168-f9f1ec02-8ec2-4025-b6be-3b58c7a83665.png)

Then choose one of the CSV files from the github. There are three important steps at this point. The first is that you alter the Table Name to ToneModels. The second is that you tick the box "Column names in first line". The third is that you head to the advanced drop down, and under "Conflict Strategy" select either "Ignore Row" or "Replace Existing Row". This is so that if you already have some of the models in your library the program doesn't freak out, SQL entries need to be unique. So if after the import you see a couple errors, don't worry that's normal, it just means you had a few duplicates.

![image](https://user-images.githubusercontent.com/116271180/197087964-2224ae98-21c6-4e7e-8fe1-6a36b9b794d7.png)

If you named the Table Name correctly you should see this dialogue, if you don't, you probably mis-typed the table name.

![image](https://user-images.githubusercontent.com/116271180/197087989-3ad4b589-841c-4baf-a9fb-25721ed92e9c.png)

Hit yes to all, if you head over to the Browse Data tab and select ToneModels, you should now see you have over 2000 models. Once you're satisfied all of the models have been imported correctly hit the "Write Changes" button at the top button bar and that's it you're done. Close SQLite, then you can open ToneX. It's normal for it to take a little while for ToneX to open as it reads the Library.db 

![image](https://user-images.githubusercontent.com/116271180/197088052-61106673-9a7c-4cb1-a04c-9710f2249769.png)

These files are an exhaustive list of the models between the dates specified, I reccomend opening them in excel or similar before you import them to weed out models you wouldn't be interested in. For instance I deleted all the entries with "Fractal", or "Helix" in their model name. I will try to update this repo periodically with new models.
