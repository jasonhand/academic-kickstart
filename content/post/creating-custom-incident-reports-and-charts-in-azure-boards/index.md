---
title: Creating Custom Incident Reports and Charts in Azure Boards
date: 2020-03-24
image:
  placement: 3
profile: false
tags: ["incidents", "tracking", "azure", "boards", "reports", "charts"]
editable: true
---

For the most part, incidents are unique.

Therefore the lessons learned will vary from problem to problem. However, it's helpful to spot trends in response efforts to both identify what is working and what needs improvement.

It's also helpful for engineering teams to have a sense of how frequent problems are arising and how quickly they are addressed and resolved.

When tracking incidents using Azure Boards, it's quite simple to build reports and charts provide a high level snapshot of incident management efforts.

## Create a Query

**1.** Select the **Queries** option in the left navigation
![](queries.png)

**2.** Customize the query

Select the  clauses, fields, and values of interest to easily build queries and report back information such as *"Show me **ANY** incident"* in this example.
![](new-query.png)

You'll see the results at the bottom of the screen. In our case we only have two incidents. One is **resolved** and one is **acknowledged**.

**3.** Save the query

Press the **Save query** menu option and give it a name such as **"All Incidents"**.

![](save-query.gif)

##  Create a Graph

To create visualizations of the queries, begin by changing to the **Charts** option.

**1.** Click on **Charts**
![](charts.png)

**2.** Click on **New Charts**
![](new-chart.png)

**3.** Configure the chart

Choose the type of chart you want to use (Pie in this example). Give the chart a name, such as "All Incidents - Chart". Choose how you want the data grouped, like "State" (**New Incident, Resolved, Acknowledged, etc.**)

Choose a color to represent the data and press Ok.
![](configure-chart.png)

Now you have a high level visual to communicate the state of incidents.

![](chart-view.png)

Now that we've discussed ways to help track the response of an incident, let's take a moment to discuss ways of [Improving the Remediation of Incidents](/post/improving-the-remediation-of-incidents/).