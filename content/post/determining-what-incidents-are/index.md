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

[Exploring Subjectivity of Incidents](/post/exploring-subjectivity-of-incidents/)