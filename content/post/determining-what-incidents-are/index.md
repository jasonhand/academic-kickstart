---
title: Determining What Incidents Are
date: 2020-03-05
image:
  placement: 3
profile: false
tags: ["incidents", "on-call"]
editable: true
---

If you search online for "Incident Response" a majority of what you'll find is information related to security threats and breaches. What doesn't show up in the results is stuff about how to properly respond to threats related to something else entirely. 

How should a business respond to technical challenges and failures as they come up? The ones that affect reliability concerns such as availability, latency, correctness, and others. What happens when service level expectations are breached and it's time for a human to get involved?

Services such as VictorOps, PagerDuty, and others provide "on-call" solutions as well as documentation and best practices regarding this type of incident management. Service Now has opinions as well but the language is aimed more for those who follow ITSM guidance regarding service management. Ticketing with a tiered support structure doesn't provide the fasted path to uptime for many companies however.

In the devops and web operations space, the idea of anyone but the engineers building the system responding to customer impacting problems is completely unacceptable. Irresponsible even. Time is of the essence and those who helped build the applications and underlying infrastructure are the best suited to maintain it's health and upgrades in a production environment.

Exactly when an engineer should be expected to take action is why we need to define what we mean by an incident.

We can all agree that an incident is a “**service disruption**” - something that is affecting our user's ability to use the services they have come to rely on.

That's a given. However, there are other things about incidents that are often overlooked or never considered. For example incidents are commonly subjective, feared, and unexpected

## Subjective

If you ask engineers across different organizations and industries, you will get many different answers about what an incident is.

Sometimes it is only when a customer is affected.

Others will label disruptions as incidents even if a customer never experienced a thing.

Subjectivity is an unfortunate property of incidents in a lot of cases, even when it comes to identifying severity levels.

## Feared  

In some cases, we downplay the significance of an outage ... or worse ... intentionally mis-label or not report a disruption in service for fear of reprimand.

Historically, we have felt that incidents reflected poorly in several areas of our engineering efforts and the organization.  

It has not been until more recently through many of the conversations around devops and site reliability engineering, that we are starting to rethink incidents and now view them as opportunities to learn and improve our systems.

## Unexpected

In other words ... unplanned Work

Most of what we as engineers and technologists do is planned work.  

We spend a lot of time and effort understanding the work in front of us.  

We calculate story points.  We plan sprints. We have a pretty good idea on what we are supposed to be working on.

So, when an incident occurs, it is disruptive. It is... unplanned work.

Often, we view this as a terrible thing, but in reality, incidents are actually “investments” in supplying the value we are trying to deliver to end users.

We just need to change how we look at incidents.

Next we'll discuss the full lifecycle of an incident. From detection to analysis and everything in between. When we start to view incidents through a new lense and begin analyzing for opportunities to learn, you'll begin to see your systems for what they are and why having a response plan in place makes sense.

## Resources

[MS Learn: Improve Incident Response with Alerting in Azure](https://docs.microsoft.com/en-us/learn/modules/incident-response-with-alerting-on-azure/)

## Next steps

[Understanding the Full Lifecycle of An Incident](/post/understanding-the-full-lifecycle-of-an-incident)