*NOTE:* This file is a template that you can use to create the README for your project. The *TODO* comments below will highlight the information you should be sure to include.


# Operationalizing Machine Learning
Project Overview:
In this project, a AutoMLpipeline was developed to deploy and cosume the cloud-based machine learning production model using Bank Marketing datset through RestAPI endpoint.

## Architectural Diagram
<img width="668" alt="Screen Shot 2022-12-31 at 2 53 13 PM" src="https://github.optum.com/storage/user/7541/files/475da4c9-a8e3-4720-8a16-b89f69a233e6">

Reference from this URL:
https://learn.udacity.com/nanodegrees/nd00333/parts/cd0601/lessons/603ad727-5d5f-4c1f-b5ac-ccdfbb6b2c6e/concepts/20394f49-3bc9-44f4-9283-82d12ce97583


## Key Steps
The following are the key steps performed during this project.

Authentication - Service Prinical cannot be created in the environment.Skipped this step.

Automated ML Experiment - Created an AutoMl experiment, configured a compute cluster, and used that cluster to run the experiment.
<img width="1770" alt="Registered Datasets" src="https://github.optum.com/storage/user/7541/files/46249a93-f246-44d6-989b-3ef6ec204bc3">
<img width="1787" alt="AutoML Completed Experiment" src="https://github.optum.com/storage/user/7541/files/bd772408-e900-4718-a5b1-e48123f377e0">


Deploy the best model - From all the models available,Best model with highest accuracy and Explanation for the given Bank Marketing dataset is taken.
<img width="1785" alt="BestModel from Completed Experiment" src="https://github.optum.com/storage/user/7541/files/74af65f1-5f83-4156-abab-8e79b927c76b">

Enable logging - Application Insights is used to collect Metrics and application Telemetry data, which includes application activities and health,Application Insights can also be used to collect and store application trace logging data.Application Insights is enabled through either Auto-Instrumentation (agent) or by adding the Application Insights SDK to your application code.
<img width="1240" alt="Applications Insights Endpoint" src="https://github.optum.com/storage/user/7541/files/786a07ae-b928-41c6-841b-fa8e6a5f8d25">
<img width="1346" alt="Run Details Logs script - I " src="https://github.optum.com/storage/user/7541/files/2b255d39-82bb-4e81-bb4e-348813e379ae">
<img width="1348" alt="Run Details Logs script - II" src="https://github.optum.com/storage/user/7541/files/37ff24fa-0f28-4fdc-923b-bb8a2c0a9fac">

Swagger Documentation: Swagger helps users build, document, test and consume RESTful web services.Azure provides a swagger.json that is used to create a web site that documents the HTTP endpoint for a deployed model.
Ran both swagger.sh and serve.py to get Docker running locally serving Swaggerto interact with the deployed model Documentation. http://localhost:8000/swagger.json providing the swagger document and specifics of the example model

<img width="1779" alt="Swagger Details" src="https://github.optum.com/storage/user/7541/files/46b685a2-ae0a-46f6-a32f-0fab5077029d">
<img width="1609" alt="Swagger Response" src="https://github.optum.com/storage/user/7541/files/83d498e4-20db-4714-b235-5f4702d52263">

Consume model endpoints: An HTTP API is a URL that is exposed over the network so that interaction with a trained model can happen via HTTP requests such as GET and POST.
<img width="1760" alt="Endpoint Model JSON Output" src="https://github.optum.com/storage/user/7541/files/cfe9ab80-71f4-40c3-81d1-bda88e47414a">
<img width="1788" alt="Benchmark run details - I " src="https://github.optum.com/storage/user/7541/files/727c9eb8-25a2-4219-b79b-a3352764dc20">
<img width="659" alt="Benchmark run details - II " src="https://github.optum.com/storage/user/7541/files/49b17e13-051f-427a-9067-cfbfda986603">


Create and publish a pipeline:Publishing the pipeline enables a REST endpoint to rerun the pipeline from any HTTP library on any platform.
<img width="1779" alt="Pipeline Creation" src="https://github.optum.com/storage/user/7541/files/dfca1355-3eb1-4f67-97b7-b0135b4fa851">
<img width="1161" alt="Pipeline Endpoint" src="https://github.optum.com/storage/user/7541/files/d4138812-b4df-43df-9607-94257342e26b">
<img width="883" alt="Published Pipeline Overview" src="https://github.optum.com/storage/user/7541/files/5271a9a4-5e4a-498f-a6c6-7fac938e849d">
<img width="1350" alt="Bankmarketing Dataset" src="https://github.optum.com/storage/user/7541/files/145c309a-f1f1-4899-8d5f-f3500354f6a5">
<img width="1331" alt="RundetailsWidget - I  " src="https://github.optum.com/storage/user/7541/files/5b86af94-1c91-40c2-89ff-d0ef0aede812">
<img width="1345" alt="RunDetails Widget - II" src="https://github.optum.com/storage/user/7541/files/d34b0c2d-71f1-4a3a-ae93-2db6c3468eb2">


## Screen Recording
*TODO* Provide a link to a screen recording of the project in action. Remember that the screencast should demonstrate:

https://youtu.be/X3DDNH1sXmU

## Standout Suggestions
*TODO (Optional):* This is where you can provide information about any standout suggestions that you have attempted.
