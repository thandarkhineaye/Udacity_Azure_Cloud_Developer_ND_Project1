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
For this, I used Azure cost estimation calculator for my web app.
Currently, I am in Japan, so I used Japan yen for currency.
The following are the estimation and comparison for App Service and Virtual machine monthly.

Estimation for using App Service:
------------------------------------------------------------------------------------------------------				
Service type	       |Region	    |Description	                     |Estimated monthly cost
Azure SQL Database		Japan East	 Single Database,Basic Tier            ¥619.67
App Service		        Japan East	 Basic Tier; Linux OS	               ¥1,553.44
Storage Accounts		Japan East	 Block Blob Storage                    ¥2,356.48
Support			                     Support	                           ¥0.00
			                         Licensing Program	                   Microsoft Online Services Agreement
			                         Total	                               ¥4,529.59
------------------------------------------------------------------------------------------------------	

Estimation for using Virtual Machine service:	
------------------------------------------------------------------------------------------------------				
Service type	       |Region	    |Description	                    |Estimated monthly cost
Azure SQL Database		Japan East	 Single Database,Basic Tier            ¥619.67
Virtual Machines		Japan East	 Basic Tier; Linux OS	               ¥1,804.32
Storage Accounts		Japan East	 1 A0 ; Linux – Ubuntu; Pay as you go; ¥2,356.48
Support			                     Support	                           ¥0.00
			                         Licensing Program	                   Microsoft Online Services Agreement
                                     Total	                               ¥4,780.47
------------------------------------------------------------------------------------------------------	

As for me, The development of app is much simpler and faster in Azure App Service.
Azure App Services do not offer Pay-as-you-Go but it was still flexisible for me.
I want to deploy with github this time, that's why I chose App service to deploy this project.

Deployed URL: http://udacityndproject1.azurewebsites.net/home