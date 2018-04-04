# Watson Studio: Use deep learning for image classification

## Mimmitkoodaa workshop 

![](/screenshots/PictureX.png?raw=true)

#### Pre-requisites:
  - IBM Cloud Account :cloud: -  www.bluemix.net

  
## Step 1: Set up the environment on IBM Cloud

Login to www.bluemix.net. If you are entering for the first time you will see something similar to the image below, your application and services dahsboard will be empty.

![](/screenshots/Picture1.png?raw=true)

In this lab we will use Watson Studio, a platform where you can create and manage machine & deep learning  workflows required  to infuse AI to drive innovation. It provides a suite of tools for data scientists, application developers and subject matter  experts to collaboratively and  easily work with data and use that data to build, train and deploy  models  at scale.

![](/screenshots/Picture0.png?raw=true)

Let's go to the catalog by clicking on the button on the right top corder and find Watson Studio, which it is located under the Watson category.

![](/screenshots/Picture2.png?raw=true)

Click on the icon and give your service a name. 
Make sure you have the correct region and space where you want to create your service and click on create.

![](/screenshots/Picture3.png?raw=true)

Now, let's enter Watson Studio. Click on the Get Started button. 

![](/screenshots/Picture4.png?raw=true)

This will open a new tab. Now we are going to create a new project. Click on the new project icon. 

![](/screenshots/Picture5.png?raw=true)

Select complete project and click OK.

![](/screenshots/Picture6.png?raw=true)

Give your project a name and a description. 

![](/screenshots/Picture7.png?raw=true)

Now, on le right side you will see that Object Storage is needed. Click on Add - this will open another tab.

    IBM Cloud Object Storage is a highly scalable cloud storage service, designed for high durability, resiliency and security. Store, manage and access your data via our self-service portal and RESTful APIs. Connect applications directly to Cloud Object Storage use other IBM Cloud Services with your data.

Select the New tab and Lite Plan for your object storage service, then click on create. 

![](/screenshots/Picture8.png?raw=true)

![](/screenshots/Picture9.png?raw=true)

Confirm the creation of the service. 

![](/screenshots/Picture10.png?raw=true)

If you don't see your service added to your project click on Refresh and then it should appear. 

![](/screenshots/Picture11.png?raw=true)

Now click on create. 

![](/screenshots/Picture12.png?raw=true)



**1. Apache Spark** 

Apache Spark is an open source cluster computing framework optimized for extremely fast and large scale data processing, which you can access via the newly integrated notebook interface IBM Analytics for Apache Spark. You can connect to your existing data sources or take advantage of the on-demand big data optimization of Object Storage. Spark plans are based on the maximum number of executors available to process your analytic jobs. Executors exist only as long as they're needed for processing, so you're charged only for processing done.

 


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

In Watson Studio you can create a machine learning model by using the model builder, the flow editor, or a notebook to prepare data, train the model, and deploy the model. In this example we will use a Jupyter Notebook.

Next click on the Assets tab and go to the Notebooks section. Click on add new Notebook. 

## IMAGE
![](/screenshots/Picture16.png?raw=true)

## IMAGE

![](/screenshots/Picture17.png?raw=true)

We will not start our Notebook from scratch, so we will import the notebook located in this repository. 
Click on Notebook from URL and give your notebook a name. For example OpenCV playground. In the notebook URL paste:

     https://github.com/sandra-calvo/mimmitkoodaa-datascience/blob/master/Use%20deep%20learning%20for%20image%20classification.ipynb

And finally click on Create. 

## IMAGE 


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

## Step 6: Run the Notebook

In order to run the notebook you can click on the Run icon and go thought the notebook cell by cell, or you can click on the Cell menu and click on Run All. 


## Summary

In this lab we used a python Jupyter notebook to use analyse images with hand written numbers using deep learning. 




