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

## What alerts are – and aren’t

To understand why alerting can create a problem, you need to think about the
purpose of alerts and how they differ from other monitoring components.

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

If the event is something that the system can handle through automated
processes, such as scaling resources within a preset limit, an alert is not
necessary. A simple line in a log should suffice.

## Create actionable alerts

To create effective actionable alerts, you must understand their components and
characteristics. Actionable alerts have:

-   Simplicity

-   Scope

-   Context

Simplicity is self-explanatory: make your alerts easy for you and others to
understand, even if you’re reading them after being awakened at 2:00 a.m. Scope
and context should be included in the content of the alert.

Let’s look at some elements that an actionable alert should always include:

-   **The source:** information about where the alert is coming from. Many
    organizations have multiple monitoring systems in use at any one time and a
    large number of interconnected systems. It can save someone a tremendous
    amount of time if the alert says "This alert for payroll system thx-1138 is
    coming from Azure monitor subscription prod."

-   **The problem:** information about what expectation has been violated. For
    example, "This server has been returning an error 30% of the time when it
    should have been returning errors less than 1% of the time."

-   **Impact and scope:** information about the effect or impact the situation
    has had or potentially will have and the scope of that impact (ideally,
    stated from the customer’s point of view).

-   **Recommended action:** if possible, the alert should include what the
    person responding should do next, even if that is a pointer to a
    troubleshooting guide or some other documentation to find help in diagnosing
    and remediating this problem.

Including such helpful context will make operations practices around monitoring
more sustainable and make responding to alerts easier.

[Determining What Incidents Are](/post/determining-what-incidents-are/)
