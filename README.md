# Watson Studio: Playing with OpenCV 
  (Open Source Computer Vision)
## Mimmitkoodaa workshop 


#### Pre-requisites:
  - IBM Cloud Account -  www.bluemix.net

  
## Step 1: Set up the environment on IBM Cloud

Login to www.bluemix.net and create the following services:

    - Cloud Object Storage
    - Apache Spark

In order to do so, go to the Catalog find the wanted service. 

![](/screenshots/Picture3.png?raw=true)

**1. Apache Spark** 

Apache Spark is an open source cluster computing framework optimized for extremely fast and large scale data processing, which you can access via the newly integrated notebook interface IBM Analytics for Apache Spark. You can connect to your existing data sources or take advantage of the on-demand big data optimization of Object Storage. Spark plans are based on the maximum number of executors available to process your analytic jobs. Executors exist only as long as they're needed for processing, so you're charged only for processing done.

Go back to the Catalog and repeat the process for Apache Spark also located under Data & Analytics
![](/screenshots/Picture5.png?raw=true)

Make sure you have the correct region and space where you want to create your service and click on create.
 
![](/screenshots/Picture8.png?raw=true)

**2. Cloud Object Storage** 

IBM Cloud Object Storage is a highly scalable cloud storage service, designed for high durability, resiliency and security. Store, manage and access your data via our self-service portal and RESTful APIs. Connect applications directly to Cloud Object Storage use other IBM Cloud Services with your data.

Go back to the Catalog and repeat the process for Cloud Object Storage, located under Storage.
![](/screenshots/Picture6.png?raw=true)

 Make sure you have the correct region and space where you want to create your service and click on create.
 
![](/screenshots/Picture9.png?raw=true)

Once you have created the three services click on the IBM Cloud logo on the top left corner to go to your Dashboard. 

![](/screenshots/Picture10.png?raw=true)

Listed you will find the needed services as shown in the image.

![](/screenshots/Picture11.png?raw=true)

## Step 2: Configure Watson Studio

Go to https://eu-gb.datascience.ibm.com to access IBM Watson Studio. 

![](/screenshots/Picture1.png?raw=true)

Sign in using your IBM Cloud credentials. 

First time you log in the service will prompt a window with you account information. Confirm your information by clicking on Continue.

![](/screenshots/Picture12.png?raw=true)

After few seconds your Watson Studio environment will be ready. Click on Done. 

![](/screenshots/Picture13.png?raw=true)

## Step 3: Create a project 

Click on New Project.

![](/screenshots/Picture14.png?raw=true)

Give the project a name and connect with your Spark and Object Storage instances. You should see the services you created in Step 1. 

![](/screenshots/Picture15.png?raw=true)

Then click on Create and your project will be ready! 

Go to the Settings tab and confirm that your project is connected to your Spark and Object Storage services created in Step 1.

![](/screenshots/Picture15.png?raw=true)

![](/screenshots/Picture30.png?raw=true)

If you are missing a service click on add new service, from existing and select from the list your service.

  ![](/screenshots/Picture31.png?raw=true)

## Step 4: Add data & import the Jupyter Notebook

You can create a machine learning model by using the model builder, the flow editor, or a notebook to prepare data, train the model, and deploy the model. In this example we will use the model builder. 

Next click on the Assets tab and go to the Notebooks section. Click on add new Notebook. 

## IMAGE
![](/screenshots/Picture16.png?raw=true)

## IMAGE

![](/screenshots/Picture17.png?raw=true)

We will not start our Notebook from scratch, so we will import the notebook located in this repository. 
Click on Notebook from URL and give your notebook a name. For example OpenCV playground. In the notebook URL paste:

## URL 

And finally click on Create. 

## IMAGE 

![](/screenshots/Picture18.png?raw=true)



Let's add some data! Download the test image Image.png file from this repository and click on Add data assets. 

![](/screenshots/Picture19.png?raw=true)

Browse for the png file and open it. Once it finished loading you will see it in the data assets.

![](/screenshots/Picture20.png?raw=true)

Now we have the image we are going to analyse and the notebook containing all the necessary libraries and algorithms to do so.

## Step 5: Access the Notebook

Click on the notebook you just created to open it. 

## IMAGE

Click on the pen icon to edit the notebook. 

## IMAGE

The only part you will need to edit is the credentials part. 

Click on the 1001 icon and you should see your Image.png listed. Under the image you should see a menu with the following options: 
## IMAGE

Click on Insert credentials and insert them in the second shell as shown in the image

## IMAGE

Now you can run your notebook and use different techniques to analyse and modify the given image. 


## Summary

In this lab we used a basic Jupyter notebook with OpenCV to analyse an image. 




