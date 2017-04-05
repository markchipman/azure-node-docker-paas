# Azure Resource Manager Template

## Overview

Use supplied [azuredeploy.json](azuredeploy.json) template to deploy the resources we need into Azure. An easy way to do this is via the Azure portal, simply click this button:  

<button style='padding:10px; font-size:18px; background-color: #0072C6; border:none; border-radius: 5px; color: white'>Deploy to Azure</button>

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fbenc-uk%2Fazure-node-docker-paas%2Fmaster%2Farm%2Fazuredeploy.json" target="_blank"><img src="http://azuredeploy.net/deploybutton.png"/></a>

## Resources Deployed
* Azure Container Registry
* Linux App Service Plan
* Linux Web App
* Storage Account

## Parameters
The template will prompt you for several parameters:
* `siteName` : The name of your web app, **Note: this must be globally unique!** 
* `registryName` : The name of your docker registry, **Note: this must be globally unique!** 
* `dockerImageName` : The name of your application Docker image 
* `dockerImagePort` : Port your application listens on