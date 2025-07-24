The purpose of this repo - 
Functional requirments - 
User logins to the app -  Oauth
User sees two options - scan for medicine or scan for prescription 
In scan medicine flow user gets  {medicine_name, diseases, similar_medicines,salts_info} nosql db cz read heavy
In scan prescription- opens camera scan docs and make a db entry allow user to correct and save into archive db — schema decide later. Same nosql check postgres too
In scan medicine - ocr-> converts to text ->llm search(text) store in a central db if the info already there serve from there. 
User dashboards 2 kinds - medicine archival and prescription archival 1 year data retention could be there opt. 
Delete option in dashboard 
Download /share option
Personal portfolio 




Non-functional requirements 
Availability- user past history or normal usability 
Durability- data should be saved on client

One question to check later  - how to save data on client if the user deletes the app. Probably store the data on server but then the server shouldn’t be able to read the data 
