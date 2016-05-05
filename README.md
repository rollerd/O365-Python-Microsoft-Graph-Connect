# Office 365 Python Connect sample using Microsoft Graph

Connecting to Office 365 is the first step every app must take to start working with Office 365 services and data. This sample shows how to connect and then call one API through the Microsoft Graph API (previously called Office 365 unified API), and uses the Office Fabric UI to create an Office 365 experience.

> Note: Try out the [Get started with Office 365 APIs](http://dev.office.com/getting-started/office365apis?platform=option-python#setup) page which simplifies registration so you can get this sample running faster.

![Office 365 Python Connect sample screenshot](./README assets/screenshot.PNG)

## Prerequisites

To use the Office 365 Python Connect sample, you need the following:
* [Python 3.4.3](https://www.python.org/downloads/)
* [Django 1.8](https://docs.djangoproject.com/en/1.8/intro/install/)
* [Requests: HTTP for Humans module](http://docs.python-requests.org/en/latest/)
* An Office 365 account. 
* A client ID (Application ID), client secret (generate a new password), and redirect URI values of an application registered in Azure: [Add a web server application in Azure](https://apps.dev.microsoft.com/#/appList)

     > Note: During the app registration process, make sure to specify **http://127.0.0.1:8000/connect/get_token/** as the **Redirect URI**.

## Configure and run the app

1. Using your favorite IDE, open **config.py** in the *connect* directory.
2. Replace *ENTER_YOUR_CLIENT_ID* with the Application ID of your registered Azure application.
3. Replace *ENTER_YOUR_SECRET* with a password generated on the **Application Secrets** area of your app in the Microsoft Application Registration Portal.
4. Set up the server by running ```python manage.py migrate```. [This command](https://docs.djangoproject.com/en/1.8/ref/django-admin/#django-admin-migrate) will synchronize the database state with the current set of migrations.
5. Start the development server by running ```python manage.py runserver```.
6. Navigate to ```http://127.0.0.1:8000/``` in your web browser.

To learn more about the sample, see [Python walkthrough on graph.microsoft.io](http://graph.microsoft.io/docs/platform/python).  

## Questions and comments

We'd love to get your feedback about the Office 365 Python Connect sample. You can send your questions and suggestions to us in the [Issues](https://github.com/OfficeDev/O365-Python-Microsoft-Graph-Connect/issues) section of this repository.

Your feedback is important to us. Connect with us on [Stack Overflow](http://stackoverflow.com/questions/tagged/office365+or+microsoftgraph). Tag your questions with [MicrosoftGraph] and [office365].
  
## Additional resources

* [Office Dev Center](http://dev.office.com/)
* [Microsoft Graph API](http://graph.microsoft.io)
* [Office UI Fabric](http://dev.office.com/fabric)

## Copyright
Copyright (c) 2015 Microsoft. All rights reserved.
