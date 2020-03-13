---
title: Monitoring For Reliability
date: 2020-03-05
profile: false
image:
  placement: 3
tags: ["monitoring", "reliability"]
editable: true
---

The world today is extremely connected.

Digital services have become so embedded in our daily lives that when they become unavailable, it often has an adverse effect on our own livelihoods. Like electricity and running water, we don't ralize our reliance on it until it's suddenly unavailable.

## Monitoring

Monitoring is a way of collecting information about what is going on in your systems so you can improve things as well as make objectively informed decisions. [Azure Monitor](https://docs.microsoft.com/en-us/azure/azure-monitor/overview/?wt_mc_id=oncalllife-blog-jahand) is an example of tooling that allows this type of collection and analysis.  

Many aspects of a system can be monitored. From the component level (CPU, Memory) to business impact and everything in between. We might gauge performance, examine security, or (in our case) evaluate and improve reliability.

## Reliability

When monitoring for reliability, we are trying to proactively manage not only the availability of a service, but many aspects of reliability.

Depending on the service and the expectations of the end user, some aspects of reliability may be more valuable than others.

{{% alert note %}}
**Exercise:** <br /> Discuss and document perceived expectations users have regarding the reliability of your service?
{{% /alert %}}

To determine what to monitor, continue with  [Examinging All Aspects of Reliability](/post/examining-all-aspects-of-reliability/)