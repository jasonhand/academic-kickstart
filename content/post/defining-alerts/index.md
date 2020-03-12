---
title: Defining Alerts
date: 2020-03-05
profile: false
image:
  placement: 3
tags: ["on-call", "alerts", "foundations"]
editable: true
---

To understand why alerting can create a problem, you need to think about the purpose of alerts and how they differ from other monitoring components.

Actionable alerts are *not*:

-   **Logs.** Alerts are not records of events; that’s the role of logs.

-   **Notifications.** Alerts are not intended to announce non-critical
    occurrences such as the completion of a software build.

-   **Heartbeats.** Alerts shouldn’t be used to document failure of a heartbeat
    signal periodically sent between two systems at regular intervals.

Actionable alerts are used for situations in which you need a human to
investigate and intervene to remediate the problem. Alerts should be
communications that something exceptional or unexpected has happened that
requires someone’s attention.

A lot of thought should be put in to how alerts are delivered and when it is necessary. [More on how to configure alerts in Azure can be found here](https://docs.microsoft.com/en-us/azure/azure-monitor/platform/alerts-overview/?wt.mc_id=oncalllife-blog-jahand).

If the event is something that the system can handle through automated
processes, such as scaling resources within a preset limit, an alert is not
necessary. A simple line in a log should suffice.

[Understanding Actionable Alerts](/post/understanding-actionable-alerts)