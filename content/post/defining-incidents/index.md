---
title: Defining Incidents
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

---

## From Microsoft's IcM Documentation

### What is an incident?

An incident is any unplanned interruption or degradation of a product or service that is causing customer impact. For example, a bad HTTP request, slow connection, security vulnerability, or customer-reported error message could constitute an incident. Every service across Microsoft has a different definition of what an incident is and when one should be triggered.

Sometimes, an incident can be severe enough to affect many different services and customers. For example, a datacenter power failure may impact dozens of Microsoft products. Severe incidents with broad impact are called outages.

Typically any customer impacting incident must be mitigated as soon as possible to minimize the customer impact. Organizations track Time-To-Mitigate (TTM) metrics for their services. For example: In Azure, TTM must be <= 30mins for any customer impacting incident.

### What is incident management?

Incident Management is the process of detecting a live-site problem with a service, creating an incident, determining the cause, restoring the service to full operation, and capturing learnings to prevent it from happening again.

### What is IcM?

IcM is the one incident management system for all Microsoft services. IcM provides tools for managing live site and on call rotations. IcM runs around the clock to keep services working across the world. Incident Types supported are "Livesite Incident", "Deployment Incident" and "Customer Reported Incidents". No additional types will be supported.

### What IcM is not?

IcM is not intended to be a ticketing solution. IcM was designed for incidents that must be mitigated within minutes to minimize the customer impact. Here are some differences:

In a ticketing solution, a ticket can take 'n' days to resolve. In IcM, incidents need to be resolved as soon as possible to minimize customer impact.

In a ticketing solution, teams might want to pause or have a count down timer for tickets. In IcM, this will not be supported because the incident has to be resolved in minutes.
In a ticketing solution, teams might want to customize the workflows. In IcM, incident workflow is fixed: Create -> Acknowledge -> Mitigate -> Resolve.

In a ticketing solution, teams might want different 'Types' and 'Sub-Types'. In IcM, only types that will be supported are "Livesite Incident", "Deployment Incident" and "Customer Reported Incidents". This is to ensure that Service teams are focused on addressing the customer impacting incidents as soon as possible.

[Exploring Subjectivity of Incidents](/post/exploring-subjectivity-of-incidents/)