# FABRIC-API-Datapipeline
Data pipeline to pull data from API and load in Fabric Lake House

In Fabric, created  data pipe line with copy data activity 

![image](https://github.com/user-attachments/assets/ec14d154-ee8c-4dcc-b3f5-ebb2f852ab2f)


Choosing the source Rest

![image](https://github.com/user-attachments/assets/3113c8bf-e843-4887-adfb-77ab2590539e)


![image](https://github.com/user-attachments/assets/e1b4fdeb-d6eb-4282-9e14-de42f1e2fb10)

Ideal url will come like below

https://weather.visualcrossing.com/VisualCrossingWebServices/rest/services/timeline/77479?unitGroup=us&key=mytoken&contentType=json

All query strings are passed using parameter in pipeline
![image](https://github.com/user-attachments/assets/744a4187-ffcd-41c9-8499-9ce867799bbe)


Preview data will come like this

![image](https://github.com/user-attachments/assets/88e3cfa6-b451-4c31-8fb4-fa5a6fe22362)


Now set destination to Lakehouse
![image](https://github.com/user-attachments/assets/bc4d82f1-963b-485f-90c4-2190ab20dd89)

Run the pipe line

![image](https://github.com/user-attachments/assets/7753baf3-b224-49f0-a95a-674652bb538a)

You can see new table created in lake house

![image](https://github.com/user-attachments/assets/03b13078-42a5-481e-845c-899c0d4b9419)

I opened it in notebook to see data






