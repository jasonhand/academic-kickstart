---
title: Monitoring For Reliability
date: 2020-03-05
profile: false
image:
  placement: 3
tags: ["monitoring", "reliability"]
editable: true
---

A reasonable level of operational awareness is necessary to effectively monitor
for reliability. Monitoring tools can help measure and improve reliability in
your organization.

You now have an expanded concept of what reliability is. Next, you need to learn
about the role monitoring plays in reaching your reliability goals.

Monitoring is a systematic and routine collection of information about
activities, events, and statuses that you can use to improve practices and make
informed decisions. In the IT world, we use monitoring for many purposes: to
gauge performance, to assess security, and in the context of this module, to
evaluate and improve reliability.

Monitoring provides the information on which the concepts of site reliability
engineering rests.

## Site Reliability Engineering

Site Reliability Engineering is an engineering discipline devoted to helping
organizations sustainably achieve the appropriate level of reliability in their
systems, services, and products.

The key concepts to take away from this definition are:

-   **Reliability.** You learned in the introductory module that there are
    multiple aspects to reliability and later in this module, you’ll examine
    each in more detail. You also learned about the importance of reliability –
    why it matters.

-   **Sustainability.** In this context, “sustainable” refers to the role of
    people in creating a sustainable operations practice. Reliable systems,
    services, products are built by people. It is crucial to the concept of SRE
    to implement an operations practice that is sustainable over time, so that
    people are able to bring their best to the job.

-   **Appropriateness.** It’s important to understand that 100% reliability
    isn’t often possible, especially in today’s complex systems with
    dependencies on other systems. 100% reliability means zero down time, which
    also means no opportunity to make any changes or improvements that could
    create some down time. Instead of striving for a goal of absolute
    reliability, determine the appropriate level of reliability for a particular
    application or service.

The role of a site reliability engineer bridges the span between operations and
development but also goes beyond DevOps, and the SRE philosophy is the basis of
a new and more efficient and effective approach to building and operating
reliable systems and applications.

## Reliability monitoring and operational awareness

Sustainably achieving an appropriate level of reliability first requires that
you know what’s going on with your systems and services. You find that out by
monitoring. Before you can effectively monitor for reliability, however, you
must have a reasonable level of operational awareness. This means you need to
understand how systems in production are functioning in order to work toward
reliability of those systems.

Today’s production environments and the paths by which we deploy systems and
applications are complex. Thus, it is not uncommon to have to do a bit of
discovery to obtain an operational awareness baseline. Some questions to ask
include:

-   What exactly is running in production?

-   Given a specific application, what are its component parts?

-   Which of those parts communicate with which other parts?

There are also some more complex factors that you’ll want to examine to give you
a better understanding of your systems and services and how to make them more
reliable.

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

The answers to all these questions will help you to build a baseline around
“normal” behavior.

## Application Insights

In the next unit, you’ll learn more about Azure Monitor and how you can use the
information it collects to evaluate and improve reliability. But first, let’s
briefly discuss a way to use one of its tools to answer some of the questions
above.

Application Insights is one of Azure Monitor’s features that can give you
insights into a particular application. It is an Azure-based service that was
made to help developers and DevOps teams understand how an app is used and how
well it performs.

Application Insights can provide you with a “big picture” that maps the
different components of your application and increase your operational awareness
to answer some of the questions asked above.

For example, you can get information about:

-   Request rates, response times, and failure rates

-   Dependency rates and information about whether external services are slowing
    your application down

-   Page views and load performance reported by users’ browsers

-   Performance data from servers

-   Diagnostics information

-   Custom events and metrics

You’ll find out more about Application Insights later in this learning path.