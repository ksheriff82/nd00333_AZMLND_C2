*NOTE:* This file is a template that you can use to create the README for your project. The *TODO* comments below will highlight the information you should be sure to include.


# Azure ML using Automation Pipeline for Bank Markerting Data set  
This project is for using the azure ML and pipeline to automate the model creatiion and publishing the pipeline and deploy model endpoints, so that the pipeline could be run on-demand and the model deployment can be automated. This helps us to automate the process, so that we can continuously improve the model as soon as we get more operational data.

## Architectural Diagram
![image](https://github.com/ksheriff82/nd00333_AZMLND_C2/assets/43680905/8f9b3ff1-4cef-491b-9b03-480b39866269)

*TODO*: Provide an architectual diagram of the project and give an introduction of each step. An architectural diagram is an image that helps visualize the flow of operations from start to finish. In this case, it has to be related to the completed project, with its various stages that are critical to the overall flow. For example, one stage for managing models could be "using Automated ML to determine the best model". 

## Key Steps
The Project started with manually uploading in the Bank Marketing Data set to Azure ML Studio
![image](https://github.com/ksheriff82/nd00333_AZMLND_C2/assets/43680905/7358ef59-3812-4313-99e5-bcc0ba5d24f1)


Use AzureML Studio to choose the best model for th AUC weighted parameter
![image](https://github.com/ksheriff82/nd00333_AZMLND_C2/assets/43680905/6e63e59d-8edf-4401-9ac2-03cb1c0f2e5e)

![image](https://github.com/ksheriff82/nd00333_AZMLND_C2/assets/43680905/776ed69d-f7cf-4a2e-ade0-831b954c0543)

Deploy the best Model, choosen by the Azure ML 

![image](https://github.com/ksheriff82/nd00333_AZMLND_C2/assets/43680905/45b643fa-9e18-4f75-bc2d-ba85ce45bb71)


Logging shown in the terminal
![image](https://github.com/ksheriff82/nd00333_AZMLND_C2/assets/43680905/ac535c3f-7dd8-4d53-a2b6-991c438ab41a)



Download the swagger file
![image](https://github.com/ksheriff82/nd00333_AZMLND_C2/assets/43680905/d51cb239-2b60-48b0-8c75-35b506803896)

Use Swagger to get the request payload json for running the model

![image](https://github.com/ksheriff82/nd00333_AZMLND_C2/assets/43680905/f8b2bda9-e710-4b6e-a16d-7374bb5e52f5)


Results from runningg endpoints.py

![image](https://github.com/ksheriff82/nd00333_AZMLND_C2/assets/43680905/b71219c6-a4ff-4d2f-ae0d-d88b69dea6d8)



Create Pipeline to Automate Model Creation
![image](https://github.com/ksheriff82/nd00333_AZMLND_C2/assets/43680905/f88d5040-8d86-4154-a4c2-c60b72597e56)

Publish Pipeline using http URL
![image](https://github.com/ksheriff82/nd00333_AZMLND_C2/assets/43680905/c385f285-4040-41c5-bdce-edf72921b48b)


## Screen Recording
https://photos.app.goo.gl/DodHATB59mK8XjQi8

## Standout Suggestions
The endpoint.py was not working as is, so I had to modify it by download the helper script provided the deployed model. It was useful for running the model for getting the results for given input. This can be be improved by providing a feedback to trigger the pipeline as we get more operational data. this would continuoly help to improve the model.
