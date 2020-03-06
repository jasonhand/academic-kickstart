---
title: Understanding the Full Lifecycle of an Incident
date: 2020-03-05
image:
  placement: 3
profile: false
tags: ["incident", "lifecycle"]
editable: true
---

If we start to think of incidents as a normal part of a system, then we can also build some formality around the patterns and practices we inevitably see when people instinctually do what they do when something goes wrong.

From the beginning of a problem to analyzing what and how things happened, we can measure them independantly of each other. By doing so, we can look for improvements in each phase.

For example, monitoring systems may be working as expected but because an alert was sent to a email distribution group, once people were aware of the alert, most assumed someone else was investigating the problem. The problem persisted for hours.

An incident can be divided into 5 phases. Detection, response, remediation, analysis, and readiness.

![Lifecycle Of An Incident](https://jhandcdn.blob.core.windows.net/blob/LifecycleOfAnIncident.png)

**Phase 1 - Detection:**
A problem has been detected through various tooling and practices

**Phase 2 - Response:**
A coordinated effort to get the right people and tooling in place to diagnose, theorize, and triage.

**Phase 3 - Remediation:**
Efforts made to change the system to either restore service or confirm theories.

**Phase 4 - Analysis:**
Post-incident retrospective exercise to understand the the full the lifecycle of the incident including the human response.

**Phase 5 - Readiness:**
Implementing knew knowledge and changes to improve and shorten the time and effects of future incidents.

Let's touch on the detection phase just a little more in depth. This is often the best place to start improving your incident response practices. Solid monitoring is the foundation of building reliable systems.

## Next steps

[The Detection Phase of an Incident](/post/incident-detection/)