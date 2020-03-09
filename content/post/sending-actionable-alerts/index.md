---
title: Sending Actionable Alerts
date: 2020-03-05
profile: false
image:
  placement: 3
tags: ["on-call", "alerts", "foundations"]
editable: true
---

Alerts play an important role in your reliability monitoring strategy, but in
order to be helpful, they must be properly constructed for situations that
warrant immediate human attention, and they should be devised with simplicity,
scope, and context in mind.

In this module, you have learned how to monitor and interact with indicators of
the reliability of your systems and create reliability goals, but there is also
an important way by which reliability interacts with you. That’s through Azure
Monitor’s log alerts feature.

It’s easy to create log alerts using Azure Monitor where the signal is a log
query in Log Analytics or Application Insights. However, there is a pitfall that
you’ll want to avoid, to prevent derailing all the effort you have put into
bringing SLIs and SLOs into your organization.

To understand this potential pitfall, review the definition of SRE:

“Site Reliability Engineering is an engineering discipline devoted to helping
organizations **sustainably** achieve the appropriate level of reliability in
their systems, services, and products.”

Alerts are designed to notify you when there is a problem with your systems.
However, when alerts are improperly configured, this can undermine your goal of
sustainability. Log alert rules are stateless; they work only on the logic that
you build into the query and they send an alert whenever the alert condition is
“true.” Thus, it’s important to put some thoughts into constructing your alerts.

[Defining Alerts](/post/defining-alerts)