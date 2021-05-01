Cloud Developer using Microsoft Azure
Udacity Nano Degree Project 1 : Deploy An Article CMS to Azure

:Project Overview
This is a simple Content Management System (CMS) for articles, where a user can log in, view published articles, and publish new articles. 
An article consists of a title, author, and body of text(to be stored in an Azure SQL Server) along with an image (to be stored in Azure Blob Storage).
Body of text and upload image are to be stored in Azure SQL Server and Blob Storage.

Components:
Python with the Flask framework(python 3.8)
SQL database(user article table)
Blob Storage(image store)

As security addition, Authentication option to Sign in with Microsoft

I think Azure VMs are more expensive to run in comparison to Azure App Service.
As for me, The development of app is much simpler and faster in Azure App Service.
Azure App Services do not offer Pay-as-you-Go but it was still flexisible for me.
I want to deploy with github this time, that's why I chose App service to deploy this project.