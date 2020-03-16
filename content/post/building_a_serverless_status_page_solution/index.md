---
title: Building a Serverless Status Page Solution
date: 2020-03-05
profile: false
image:
  placement: 3
tags: ["chatops", "devops", "communication", "collaboration", "stakeholders", "serverless", "status"]
editable: true
---

[![](https://jhandcdn.blob.core.windows.net/blob/UpdateFromTeams.gif)](https://jhandcdn.blob.core.windows.net/blob/UpdateFromTeams.gif)

### Tech Used

The brains behind this solution is an Azure Function (running Node.js) that is triggered via outgoing webhook (from Microsoft Teams). The function modifies an index.html file stored in a "web server" served from a serverless SMB file share in Azure Storage.

Users can `open`, `update`, and `close` "status updates" by invoking them from within a chat channel.

The text that follows the command will be stored and displayed on the site below the colored (Red or Green) header.

In addition to the website files, an Azure Table will be used for storing the history of each status update.
>**NOTE:** The table is not provisioned with the deployment script. It needs to be manually created in Step 2 below.

SignalR manages refreshing the client so that changes made to the HTML are immediately visible without any end user interaction.

Application Insights is used to provide observability on the operation, behavior, and usage of the solution and is "best practice" for building highly available and reliable system... which we expect from any Status Page solution.

### Prerequisites

You will need an account with the following services: 

- [Microsoft Azure](https://cda.ms/16X)
- [Microsoft Teams](https://cda.ms/17f)

---

### Deployment Instructions

The blue button below will deploy all resources needed for this solution in to the Resource Group and Azure region of your choice. The name you choose also determines the URL used to view the Status Page as well as the incoming URL used to trigger updates.

#### Steps To Deploy

**1.** Create the Azure Function app, Storage account, and SignalR Service with this button: [![Deploy to Azure](https://azuredeploy.net/deploybutton.png)](https://azuredeploy.net/)

>This will begin deploying everything needed for the solution and will provide a link to the public facing URL of the Status Page as well as a link to your new resource group where you will continue with step 2.

---

**2.** In the Azure portal, open the Storage account and add a table named `statuses`. You do not need to set any properties or add records.

![Create table](https://jhandcdn.blob.core.windows.net/blob/CreateStatusesTable.gif)

---

**3.** Navigate to the function app, and open the `teams-webhook` function. Click "Get Function URL" and copy the URL. 

**4.** Open the URL of the Function in a new tab. This is "Status Page" that will change automatically when updated. It is NOT the same as the "Get Function URL" used in the next step.

![](https://jhandcdn.blob.core.windows.net/blob/ReindeerGuidanceSystemURL.png)

---

**5.** Open Microsoft Teams and navigate to the "Apps" page of the team in which you want to create the bot. Click "Create outgoing webhook".

- Use `StatusPage` as the bot name (this is hardcoded, for now). 
- Paste in the function URL, and enter a description and press the create button.

> You will be prompted with a secret code for validating webhook calls from Teams. We currently do not use this. Close the dialog box.

[![](https://jhandcdn.blob.core.windows.net/blob/WebhookStatic.png)](https://jhandcdn.blob.core.windows.net/blob/Webhook.gif)

**6.** In Microsoft Teams, update the status page by typing `@StatusPage` to summon the bot followed by `open We are experiencing a problem. Standby for more information`

Available commands are:

```bot
        @StatusPage open [message]
        @StatusPage update [message]
        @StatusPage close [message]
        @StatusPage help`
```

---

This solution is based on the on-stage demonstrations built for Microsoft Ignite The Tour.

To learn more about the full demonstration, view the repo for "[OPS20 - Responding To Incidents](https://myignite.techcommunity.microsoft.com/sessions/82997/?WT.mc_id=oncalllife-blog-jahand)". Huge Thanks to [Anthony Chu](https://github.com/anthonychu) in bringing this to life.

Now, let's move on to 
[Understanding Why We Learn From Incidents](/post/understanding-why-we-learn-from-incidents/).