<h1>Cloud Developer using Microsoft Azure</h1><br>
<h3>Udacity Nano Degree Project 1 : Deploy An Article CMS to Azure</h3>

<h5>Project Overview</h5>
This is a simple Content Management System (CMS) for articles, where a user can log in, view published articles, and publish new articles. <br>
An article consists of a title, author, and body of text(to be stored in an Azure SQL Server) along with an image (to be stored in Azure Blob Storage).<br>
Body of text and upload image are to be stored in Azure SQL Server and Blob Storage.<br><br>

<h5>Components</h5>
:Python with the Flask framework(python 3.8)<br>
:SQL database(user article table)<br>
:Blob Storage(image store)<br><br>

As security addition, Authentication option to Sign in with Microsoft.<br>
I think Azure VMs are more expensive to run in comparison to Azure App Service.<br>
For this, I used Azure cost estimation calculator for my web app.<br>
Currently, I am in Japan, so I used Japan yen for currency.<br>
The following are the estimation and comparison for App Service and Virtual machine monthly.<br><br>

<b><i>Cost Estimation for using App Service:</b></i>
--------------------------------------------------------------
<table>
    <tr>
        <td>Service type</td>
        <td>Region</td>
        <td>Description</td>
        <td>Estimated monthly cost</td>
    </tr>
    <tr>
        <td>Azure SQL Database</td>
        <td>Japan East</td>
        <td>Single Database,Basic Tier</td>
        <td>¥619.67</td>
    </tr>
        <td>App Service</td>
        <td>Japan East</td>
        <td>Basic Tier; Linux OS	</td>
        <td>¥1,553.44</td>
    <tr>
        <td>Storage Accounts</td>
        <td>Japan East</td>
        <td>Block Blob Storage</td>
        <td>¥2,356.48</td>
    </tr>
    <tr>
        <td colspan="3">Licensing Program</td>
        <td>Microsoft Online Services Agreement</td>
    </tr>
    <tr>
        <td colspan="3"><b>Total</b></td>
        <td>¥4,529.59</td>
    </tr>
</table><br>
---------------------------------------------------------------	<br>
<b><i>Cost Estimation for using App Service:</b></i>
--------------------------------------------------------------
<table>
    <tr>
        <td>Service type</td>
        <td>Region</td>
        <td>Description</td>
        <td>Estimated monthly cost</td>
    </tr>
    <tr>
        <td>Azure SQL Database</td>
        <td>Japan East</td>
        <td>Single Database,Basic Tier</td>
        <td>¥619.67</td>
    </tr>
        <td>Virtual Machines</td>
        <td>Japan East</td>
        <td>Basic Tier; Linux OS	</td>
        <td>¥1,804.32</td>
    <tr>
        <td>Storage Accounts</td>
        <td>Japan East</td>
        <td>Block Blob Storage</td>
        <td>¥2,356.48</td>
    </tr>
    <tr>
        <td colspan="3">Licensing Program</td>
        <td>Microsoft Online Services Agreement</td>
    </tr>
    <tr>
        <td colspan="3"><b>Total</b></td>
        <td>¥4,780.47</td>
    </tr>
</table>
---------------------------------------------------------------	

Estimation for using Virtual Machine service:	
---------------------------------------------------------------		
Service type	       |Region	    |Description	                    |Estimated monthly cost
Azure SQL Database		Japan East	 Single Database,Basic Tier            ¥619.67
Virtual Machines		Japan East	 Basic Tier; Linux OS	               ¥1,804.32
Storage Accounts		Japan East	 1 A0 ; Linux – Ubuntu; Pay as you go; ¥2,356.48
Support			                     Support	                           ¥0.00
			                         Licensing Program	                   Microsoft Online Services Agreement
                                     Total	                               ¥4,780.47
---------------------------------------------------------------	

In my opinion, The development of app is much simpler and faster in Azure App Service.
Azure App Services do not offer Pay-as-you-Go but it was still flexible for me.
I want to deploy with github this time, that's why I chose App service to deploy this project.
