---
services: bot
platforms: nodejs
author: denniszielke
---

# Web application development with Node.js, Application Insights for Bot Framework
This sample shows you how to use the bot framework hosted on Azure Websites. 

## Running this sample
1. Deploy the arm template in arm/Website.json to azure

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fdenniszielke%2Fhellobot%2Fmaster%2Fbotsite.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>  

It will deploy the following resources
- App service
- Application Insights
- Configuration inside the app service appsettings

## Deploy this sample to Azure

1. If you haven't already, enable a git repository for your Azure Website. You can find instructions on how to do this [here](https://azure.microsoft.com/en-us/documentation/articles/web-sites-publish-source-control-git/#step4).

2. Add your Azure Website as a git remote.

		git remote add azure https://username@your-website.scm.azurewebsites.net:443/your-website.git

3. Deploy by pushing to the remote.

		git push azure master

4. In a few seconds, git will finish publishing your web application and launch a browser where you can see your handy work running in Azure!
