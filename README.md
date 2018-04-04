# Watson Studio: Use deep learning for image classification

## Mimmitkoodaa workshop 

![](/screenshots/PictureX.png?raw=true)

#### Pre-requisites:
  - IBM Cloud Account :cloud: -  www.bluemix.net

  
## Step 1: Set up the environment on IBM Cloud

Login to www.bluemix.net. If you are entering for the first time you will see something similar to the image below, your application and services dahsboard will be empty.

![](/screenshots/Picture1.png?raw=true)

In this lab we will use **Watson Studio**, a platform where you can create and manage machine & deep learning  workflows required  to infuse AI to drive innovation. It provides a suite of tools for data scientists, application developers and subject matter  experts to collaboratively and  easily work with data and use that data to build, train and deploy  models  at scale.

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

**IBM Cloud Object Storage** is a highly scalable cloud storage service, designed for high durability, resiliency and security. Store, manage and access your data via our self-service portal and RESTful APIs. Connect applications directly to Cloud Object Storage use other IBM Cloud Services with your data.

Select the New tab and Lite Plan for your object storage service, then click on create. 

![](/screenshots/Picture8.png?raw=true)

![](/screenshots/Picture9.png?raw=true)

Confirm the creation of the service. 

![](/screenshots/Picture10.png?raw=true)

If you don't see your service added to your project click on Refresh and then it should appear. Now click on create. 

![](/screenshots/Picture11.png?raw=true)

As you can see the project includes many options, assets, collaborators, deployments... feel free to explore the options before you continue with the lab. 

![](/screenshots/Picture12.png?raw=true)

Now let's add some computing power to run our algorithims. Let's go to the Settings tab. 

![](/screenshots/Picture13.png?raw=true)

Go down to Associated Services, which should be empty. Let's click on the Add a service button and Spark option. This will open a new tab. 

![](/screenshots/Picture14.png?raw=true)

**Apache Spark** is an open source cluster computing framework optimized for extremely fast and large scale data processing, which you can access via the newly integrated notebook interface IBM Analytics for Apache Spark. You can connect to your existing data sources or take advantage of the on-demand big data optimization of Object Storage. Spark plans are based on the maximum number of executors available to process your analytic jobs. Executors exist only as long as they're needed for processing, so you're charged only for processing done.

Select from the New tab the Lite plan for Spark and click on Create. 

![](/screenshots/Picture15.png?raw=true)

Confirm the creation of the service. 

![](/screenshots/Picture16.png?raw=true)

 Finally, your environment is ready! :+1:


## Step 2: Add a notebook

Click on the Add to project icon and select Notebook.

![](/screenshots/Picture17.png?raw=true)

We will not start our Notebook from scratch, so we will import the notebook located in this repository. Select From URL tab and give your notebook a name.

![](/screenshots/Picture17a.png?raw=true)

In the notebook URL paste the following URL:

     https://github.com/sandra-calvo/mimmitkoodaa-datascience/blob/master/Use%20deep%20learning%20for%20image%20classification.ipynb

As the running engine for our notebook we will use the Spark service we added in the previous step, so select your spark instance from the list. Then click on Create notebook. 

![](/screenshots/Picture18.png?raw=true)


## Step 3: Explore the Notebook

This notebook is divided in three parts: 
- Load libraries
- Access data
- Train the pattern recognition model

First we will install the necessary libraries in our project. For deep learning we will use **nolearn** library. nolearn is a Python package with utility functions for machine learning tasks.

The we will need data to train our model. MNIST (http://yann.lecun.com/exdb/mnist/) is a database of handwritten numbers. Because it uses real-world data, it is an ideal database for training neural networks and machine learning tools that use pattern recognition.
We will split the data into two data sets, one for training and one for testing. That way we can always test our model with new images the model has never seen before. In this case we will take 1/3 for testing and 2/3 for training. 

Now we are ready to train our model. The notebook shows you how to train a pattern recognition model for handwritten numbers by using the Deep Belief Network (DBN) solver. The DBN solver is trained on approximately 47,000 images each with 784 pixels (28 by 28 before vectorizing) and uses 300 hidden units to support more efficient learning rates. The ten output units correspond to each of the single digit numbers (0 - 9). The results of the learning algorithms have an accuracy of 98 percent.

Let's run the notebook and see the results!


## Step 4: Run the notebook

In order to run the notebook you can click on the Run icon and go thought the notebook cell by cell, or you can click on the Cell menu and click on Run All. 

![](/screenshots/Picture19.png?raw=true)

Note that the training part will take few minutes to run. 

Once you have run the whole notebook you can go to the end and run again the cells with the code:
        randIm()
        
        
![](/screenshots/Picture20.png?raw=true)
 
This will run a random image through our model and give us the prediction. 
As you will see the model is not perfect, it needs more training to increase accuracy. 


## Summary

In this lab we used a python Jupyter notebook to use analyse images with hand written numbers using deep learning. 




