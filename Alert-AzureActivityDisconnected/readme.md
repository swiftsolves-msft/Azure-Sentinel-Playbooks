# Alert-AzureActivityDisconnected
author: Nathan Swift

This will deploy a Azure Monitor Alert for AzureActivity Logs being disconnected from Azure Sentinel or Log Analytics Workspace. This could be indicative of an early attack stage and should be investigated immeaditly. Be sure after deployment to go to the alert in Azure Monitor and create and attach a Action Group so that you are notified when this occurs. The Caller and Callers IPAddr should also be caputred in the alert and ActivityLogs for review.

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fswiftsolves-msft%2FAzure-Sentinel-Playbooks%2Fmaster%2FAlert-AzureActivityDisconnected%2Fazuredeploy.json" target="_blank">
    <img src="https://aka.ms/deploytoazurebutton"/>
</a>
<a href="https://portal.azure.us/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fswiftsolves-msft%2FAzure-Sentinel-Playbooks%2Fmaster%2FAlert-AzureActivityDisconnected%2Fazuredeploy.json" target="_blank">
<img src="https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/deploytoazuregov.png"/>
</a>

**Additional Post Install Notes:**

After deployment go to the Alert in Azure Monitor and create and attach a Action Group for notification.
