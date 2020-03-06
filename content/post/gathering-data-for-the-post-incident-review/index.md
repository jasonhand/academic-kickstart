---
title: Gathering Data For the Post-incident Review
date: 2020-03-05
image:
  placement: 3
profile: false
tags: ["incidents", "data", "analysis"]
editable: true
---

The post-incident review process begins with the data. That includes the data in
the conversations related to the incident as well as the data collected by
monitoring systems. You can use Azure tools to collect, find, correlate, and
share the data in the course of conducting your learning review.

In this unit, you’ll learn how to go about the construction of a shared,
accurate chronology that reflects the non-linear nature of an incident.
*Non-linear* refers to the fact that incidents are almost never just a matter of
“this happened, and then that happened, then we noticed, then we did something,
and then we were done.”

As an incident occurs, develops, and plays out, different people get involved.
They notice and try different things, and some work, some don’t. If multiple
people are working at the same time, all these things can be happening
simultaneously. Thus, it’s a bit more complicated than just a straight-line
description.

To create a logical timeline, then, you need a starting point and the place to
start is with the relevant data.

## Gather the data

Before you can conduct a learning review, you first need to gather data.
Specifically, you need to collect as much of the conversation surrounding the
event as you can so you can use all of the crucial data contained in it. The
conversation among team members that happened during the outage or incident will
be one of your richest sources of information.

You also should gather from your monitoring system and other places from which
the people involved in the incident drew context. What information were they
getting from your systems when the incident was going on?

And finally, if possible, it would be helpful for you to get a better picture of
what changed just prior to and during the incident because changes are often
contributing factors when an incident occurs.

The data-gathering step has three parts:

-   **Collect the conversation.** It’s important to have a place for people to
    communicate and share what worked and what failed, what they’re hesitant to
    try, what they’ve tried in the past. This conversation between the people as
    they work through and solve the issue is your best source of learning.

-   **Determine the context.** This is done primarily through monitoring. It
    involves building a point in time to collect the data you have and correlate
    it to the event now that you’re looking back at it.

-   **Find the changes.** You do this through activity and audits logs.

## Data collection tools

There are tools that you can use to make these steps easier. Using Azure for
these systems can help make you better able to gather all this data quickly.

**Azure DevOps**

You have data already captured in the Azure DevOps Boards that includes tracking
of incidents with information about who was on call, who was assigned to the
incident, and so forth. You can also use the Azure DevOps Wiki as a centralized
way to pull in some of the pieces of information about both the incident itself
and the conversation that happened during the incident.

**Graph Explorer**

You can also use queries in Graph Explorer to programmatically find, export and
bring in the conversation that was collected inside the Teams channel that was
devoted to this specific incident.

**Dashboards, Application Insights and JSON**

You can create a dashboard in the Azure portal to correlate what the operators
were seeing to the incident itself. Application Insights give you graphs you can
add to the dashboard to visualize the information. This allows you to see your
tracked metrics side-by-side to better identify where and when the incident
happened. You can pull down the dashboard and its components using JSON, and,
for example, focus on a specific window of time and drill down to provide more
context for your investigation.

**Log Analytics and Audit Log**

You can use information here to discover changes and find the delta between
where you started and where you ended.