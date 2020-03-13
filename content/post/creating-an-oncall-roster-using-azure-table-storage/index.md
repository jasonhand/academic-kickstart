---
title: Creating an On-call Roster Using Azure Table Storage
date: 2020-03-13
profile: false
image:
  placement: 3
tags: ["on-call", "roster", "azure", "table storage"]
editable: true
---

On-call rosters allow teams to identify who is responsible for acknowledging and addressing incidents as they occur.

They are made up of the names and contact information of everyone expected to take part in the response and remediation of service disruptions.

**On-call Roster**

|Name   |Email   |Service   |On-call   |
|---|---|---|---|
|Jason Hand   |jason@xyz.com   |API   |Yes   |
|Chris Smith   |chris@xyz.com   |API   |No   |
|Lauren Jones   |lauren@xyz.com   |Mobile   |Yes   |
|Ryan Boggs   |ryan@xyz.com   |Database   |Yes   |

Depending on the make up of your teams and services, on-call rosters can remain quite simple or become extremely complex.

One simple way of creating an on-call roster to look up and contact individuals in response to a service disruption is with a basic storage table in Azure.

{{% alert note %}}
If you don't already have a [free Azure account, grab one here](https://azure.microsoft.com/?wt.mc_id=oncalllife-blog-jahand).
{{% /alert %}}


**1.** Create a new resource
From the home screen in Azure, select the option to **create a resource**.
![](create-a-resource.png)

**2.** Search for and select "**Storage Account**"

![](create-storage-account.png)

**3.** Select a **subscription**, **resource group**, etc.

Choose where you want the storage account created, what name you want to give it, as well as the type of disk and access tiers and then choose **Review & Create**, followed by **Create**.

**4.** Go to the (**Storage Account**) resource

**5.** Click on the **Tables** card
![](click-on-tables-card.png)

**6.** Click the **+ Table** option and give it a name of `oncall`

![](create-on-call-table.gif)

**7.** Click on **Storage Exploror**

**8.** Click on **Tables**, then **oncall**, then **+ Add**
![](open-oncall-table.png)

**9.** Add **entity**

The **PartitionKey** field will remain the same. Add new properties for **name**, **email**, **service**, and **oncall**. All properties should be set to a *string* type, except for **oncall**. It is a boolean. Once all fields have been added, press **Insert**.

![](add-table-entity.png)

**10.** Repeat the process for new entities
Make sure to use the same PartitionKey but a unique rowkey. Also be sure to use true or false for the oncall field.

After a couple of entries, it should look as follows.
![](on-call-table-entries.png)

That's it. You've taken your first steps towards building a basic on-call roster. This will help us identify who to initially alert when an incident occurs.

Next, we will take a look at [Establishing On-call Rotations](/post/establishing-oncall-rotations/)