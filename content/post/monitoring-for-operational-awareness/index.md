---
title: Monitoring For Operational Awareness
date: 2020-03-05
profile: false
image:
  placement: 3
tags: ["monitoring", "reliability"]
editable: true
---

Sustainably achieving an appropriate level of reliability first requires that you know what’s going on with your systems and services. You find that out by monitoring. Before you can effectively monitor for reliability, however, you must have a reasonable level of operational awareness. This means you need to
understand how systems in production are functioning in order to work toward reliability of those systems.

![](/post/monitoring-for-operational-awareness/operational-awareness.png)

Today’s production environments and the paths by which we deploy systems and applications are complex. Thus, it is not uncommon to have to do a bit of discovery to obtain an operational awareness baseline.

Some questions to ask include:

-   What exactly is running in production?

-   Given a specific application, what are its component parts?

-   Which of those parts communicate with which other parts?

There are also some more complex factors that you’ll want to examine to give you a better understanding of your systems and services and how to make them more reliable.

-   **How did the app or service perform in the past?** It’s true that “past
    performance is no guarantee of future results.” However, knowledge about
    past performance can be useful in calibrating expectations, and awareness of
    past outages can provide you with a sense of potential failure modes that
    you should incorporate into your thought processes around reliability.

-   **What is the socio-technical context?** In other words, who owns or cares
    about the service or app? How did it get deployed? Information about the
    stakeholders, as well as knowing, for example, whether it was deployed by
    hand or via an automated process can have many ramifications when we begin
    to make updates to improve reliability.

The answers to all these questions will help you to build a baseline around “normal” behavior.

[Monitoring For Reliability](/post/monitoring-for-reliability/)