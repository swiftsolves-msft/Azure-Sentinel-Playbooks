# IncidentClosed-Sync-ASCAlertDismiss
author: Nathan Swift

This Logic App will execute every hour and find any closed Sentinel incidents and will then dismiss the corresponding Azure Security Center alert. Acts as a background sync engine. 

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fswiftsolves-msft%2FAzure-Sentinel-Playbooks%2Fmaster%2FIncidentClosed-Sync-ASCAlertDismiss%2Fazuredeploy.json" target="_blank">
    <img src="https://aka.ms/deploytoazurebutton"/>
</a>
<a href="https://portal.azure.us/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fswiftsolves-msft%2FAzure-Sentinel-Playbooks%2Fmaster%2FIncidentClosed-Sync-ASCAlertDismiss%2Fazuredeploy.json" target="_blank">
<img src="https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/deploytoazuregov.png"/>
</a>

**Additional Post Install Notes:**

The Logic App uses a Managed System Identity to authenticate and authorize against management.azure.com to dismiss the ASC Alert. Be sure to turn on the System Assigned Identity in the Logic App. 

Assign RBAC 'Security Admin' role to the Logic App at the Subscription level.