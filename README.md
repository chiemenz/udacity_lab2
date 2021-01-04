## Udacity Project 

The Goal of this project was to find and deploy a well performing classification model which can predict the 
success of a marketing campaign based on customer input features. The features of an example customer are shown 
bellow:

 {
            "age": 48,
            "campaign": 1,
            "cons.conf.idx": -36.2,
            "cons.price.idx": 92.893,
            "contact": "cellular",
            "day_of_week": "mon",
            "default": "no",
            "duration": 971,
            "education": "university.degree",
            "emp.var.rate": -1.8,
            "euribor3m": 1.299,
            "housing": "no",
            "job": "blue-collar",
            "loan": "yes",
            "marital": "married",
            "month": "may",
            "nr.employed": 5099.1,
            "pdays": 999,
            "poutcome": "failure",
            "previous": 1
5

The best model was a **VotingEnsemble** classifier with a weighted area under the curve score **(weighted AUC) of 0.94794**
This model was deployed to a Container Instance with Authentication. 


Result of **python endpoint.py** [Consume Endpoint Result](https://github.com/chiemenz/udacity_lab2/blob/master/ConsumeEndpointResult.PNG)
The logs.py output can be seen here [Log Outputs](https://github.com/chiemenz/udacity_lab2/blob/master/LogsOutput.PNG)


For the best model you can see that it has been both registered and deployed [Best Deployed Model](https://github.com/chiemenz/udacity_lab2/blob/master/best_deployed_model.PNG)

The BankMarketingAutoML Pipeline Endpoint is active [ActivePipelineEndpoint](https://github.com/chiemenz/udacity_lab2/blob/master/ActivePipelineEndpoint.PNG)


Application Insights is enabled for the deployed marketingmodel[Application Insights Enabled](https://github.com/chiemenz/udacity_lab2/blob/master/ApplicationInsightsEnabled.PNG)
The AutoML Experiment Run has been completed [AutoML completed](https://github.com/chiemenz/udacity_lab2/blob/master/AutoMLExpCompleted.PNG)
THe results of the AutoML run are enlisted here [Best Model Experiment](https://github.com/chiemenz/udacity_lab2/blob/master/BestModelExperiment.PNG)

An AutML pipeline has been started by HTTP post request of the Published pipeline [AutoML run by POST REQUEST](https://github.com/chiemenz/udacity_lab2/blob/master/AutoMLRunByPostRequest.PNG)

A pipeline has been scheduled with a 4 hour interval [Create Scheduled Pipeline](https://github.com/chiemenz/udacity_lab2/blob/master/CreateScheduledPipeline.PNG)


Since the default python commands for running a local Swagger container were not succeeding a python flask app was created 
instead and the "swagger.json" was hosted by means of this flask swagger UI app instead (https://github.com/chiemenz/udacity_lab2/blob/master/app_project.zip)

The model POST and GET endpoints are documented with Swagger [Model Swagger Docu](https://github.com/chiemenz/udacity_lab2/blob/master/ModelSwaggerUI.PNG) & [Model Swagger Input Params](https://github.com/chiemenz/udacity_lab2/blob/master/ModelExampleSwaggerValues.PNG)


A Pipeline was created [Pipeline Creation](https://github.com/chiemenz/udacity_lab2/blob/master/PipelineCreated.PNG)
The Pipeline was published [Pipeline Published](https://github.com/chiemenz/udacity_lab2/blob/master/PublishedPipeline.PNG)
A queued Pipeline by Post request [QueuedPipelineRunByPostRequest](https://github.com/chiemenz/udacity_lab2/blob/master/QueuedPipelineRunByPostRequest.PNG)
Registered Bank Marketing Dataset [RegisteredBankMarketingSet](https://github.com/chiemenz/udacity_lab2/blob/master/RegisteredBankMarketingSet.PNG)
Run details of the pipeline step [RunDetailsPipelineSteps](https://github.com/chiemenz/udacity_lab2/blob/master/RunDetailsPipelineSteps.PNG)
A Swagger Container is running on Port 4030 [SwaggerContainerRunningOnPort4030](https://github.com/chiemenz/udacity_lab2/blob/master/SwaggerContainerRunningOnPort4030.PNG)



In this project, you will following the below steps:

    Authentication
    Automated ML Experiment
    Deploy the best model
    Enable logging
    Swagger Documentation
    Consume model endpoints
    Create and publish a pipeline
    Documentation
,



Here is the link to the brief video showing:

* 1.) The deployed model endpoint
* 2.) How to consume the deployed model with the endpoint.py script
* 3.) The AutoML model ==> best selected model
* 4.) The Published Pipeline

[Link to Video](https://www.loom.com/share/19379c75f6bf4158a697814dd1465fbf)
