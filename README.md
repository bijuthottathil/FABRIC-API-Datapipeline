# FABRIC-API-Datapipeline

![image](https://github.com/user-attachments/assets/db3b9c7f-8980-4e2e-863c-5e0772758a74)

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

Next step, trying to remove some unwnated column using Dataflow Gen2

![image](https://github.com/user-attachments/assets/51492ac3-06a4-4f83-a1f7-35a688851470)

Published and setting a destination . 


Here I am publishing this dataflow output to a data warehouse existing in my Fabric workspace

![image](https://github.com/user-attachments/assets/4d58b5f3-7d0a-4e39-a398-2aa4f1bf11c3)


Here we have options to change datatypes 

![image](https://github.com/user-attachments/assets/e0599bb9-e496-4b4b-840d-cf5eebc686fd)


Now I am in warehouse. you can see new table related to Weatherdata is generated

![image](https://github.com/user-attachments/assets/cedf04a3-0ae2-4c85-8b21-4edc15726dcd)


![image](https://github.com/user-attachments/assets/0383705f-8143-4608-a2b6-a2601c1b77d2)


I added dataflow activity in the existing pipeline to push cleaned data from Dataflow to Data ware house

![image](https://github.com/user-attachments/assets/0642be36-8bd3-4002-8e09-eee661a9f3df)

and you can see table generated in Warehouse

![image](https://github.com/user-attachments/assets/121f8ade-e0bf-49c5-af2d-c0c987cc2a8f)


