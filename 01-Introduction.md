# Lab 1: Implement Computer Vision Capabilities

## Introduction

This hands-on lab guides you through creating an intelligent console application from end-to-end using Cognitive Services (specifically the Computer Vision API). We use the ImageProcessing portable class library (PCL), discussing its contents and how to use it in your own applications.


# Lab 1: Meeting the Technical Requirements

## Lab 1.1: Setting technology, environments and keys

This lab is meant for an Artificial Intelligence (AI) Engineer or an AI Developer on Azure. To ensure you have time to work through the exercises, there are certain requirements to meet before starting the labs for this course.

You should ideally have some previous exposure to Visual Studio. We will be using it for everything we are building in the labs, so you should be familiar with [how to use it](https://docs.microsoft.com/en-us/visualstudio/ide/visual-studio-ide) to create applications. Additionally, this is not a class where we teach code or development. We assume you have some familiarity with C# (intermediate level - you can learn [here](https://mva.microsoft.com/en-us/training-courses/c-fundamentals-for-absolute-beginners-16169?l=Lvld4EQIC_2706218949) and [here](https://docs.microsoft.com/en-us/dotnet/csharp/quick-starts/)), but you do not know how to implement solutions with Cognitive Services.

### Account Setup

> **Note** You can use different environments for completing this lab.  Your instructor will guide you through the necessary steps to get the environment up and running.   This could be as simple as using the computer you are logged into in the classroom or as complex as setting up a virtualized environment.

#### Setup your Azure Account:

You may activate an Azure free trial at [https://azure.microsoft.com/en-us/free/](https://azure.microsoft.com/en-us/free/).

If you have been given an Azure Pass to complete this lab, you may go to [http://www.microsoftazurepass.com/](http://www.microsoftazurepass.com/) to activate it.  Please follow the instructions at [https://www.microsoftazurepass.com/howto](https://www.microsoftazurepass.com/howto), which document the activation process.  A Microsoft account may have **one free trial** on Azure and one Azure Pass associated with it, so if you have already activated an Azure Pass on your Microsoft account, you will need to use the free trial or use another Microsoft account.

### Environment Setup

These labs are intended to be used with the .NET Framework using [Visual Studio 2019, Community Edition](https://www.visualstudio.com/downloads/). The labs can be completed with a local computer running Visual Studio 2019 Community Edition and the required software downloads listed throughout the lab steps.

### Urls and Keys Needed

Over the course of this lab, we will collect a variety of Cognitive Services keys and storage keys. You should save all of them in a text file so you can easily access them in future labs.

>_Keys_
>
>- Cognitive Services API Url:
>- Cognitive Services API key:
>- Azure Storage Connection String:
>- Cosmos DB Url:
>- Cosmos DB Key:

> **Note** Not all of these will be populated in this lab.

### Azure Setup

In the following steps, you will configure the Azure environment for the labs that follow.

####    Cognitive Services

While the first lab focuses on the [Computer Vision](https://www.microsoft.com/cognitive-services/en-us/computer-vision-api) Cognitive Service, Microsoft Azure allows you to create a cognitive service account that spans all services, or you can elect to create a cognitive service account for an individual service.  In the following steps, you will create an account that spans all cognitive services.

1.  Open the [Azure Portal](https://portal.azure.com)

1.  Click **+ Create a Resource** and then enter **cognitive services** in the search box 

1.  Choose **Cognitive Services** from the available options, then click **Create**

> **Note** You can create specific cognitive services resources or you can create a single resource that contains all the endpoints.

1.  Type a name of your own choosing

1.  Select your subscripton and resource group

1.  For the pricing tier, select **S0**

1.  Check the confirmation checkbox

1.  Click **Create**

1.  Navigate to the new resource, click **Quick Start**

1.  Copy the **url** and the **endpoint** to your notepad

####    Azure Storage Account

1.  In the Azure Portal, click **+ Create a Resource** and then enter **storage** in the search box 

1.  Choose **Storage account** from the available options, then click **Create**

1.  Select your subscription and resource group

1.  Type a unique name for your account

1.  For the location, select the same as your resource group

1.  Performance should be **Standard**

1.  Account kind should be **StorageV2 (general purpose v2**)

1.  For replication, select **Locally-redundant storage (LRS)**

1.  Click **Review + create**

1.  Click **Create**

1.  Navigate to the new resource, click **Access Keys**

1.  Copy the **Connection string** to your notepad

1.  Select **Overview**, then click **Containers**

1.  Select **+ Container**

1.  For the name, type **images**

1.  Select **OK**

####    Cosmos DB

1.  Open the [Azure Portal](https://portal.azure.com)

1.  Click **"+ Create a Resource"** and then enter **cosmos** in the search box 

1.  Choose **Azure Cosmos DB** from the available options.  

1.  Click **Create**

1.  Select your subscription and resource group

1.  Type a unique account name, select a location that matches your resource group

1.  Click **Review + create**

1.  Click **Create**

1.  Navigate to the new resource, under **Settings**, select **Keys**

1.  Copy the **URI** and the **PRIMARY KEY** to your notepad


## Next Steps

-   [Implement Computer Vision](../02-Implement_Computer_Vision.md)