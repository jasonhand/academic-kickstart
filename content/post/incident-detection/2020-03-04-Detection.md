---
title: Incident Detection
date: 2020-03-05
math: true
diagram: true
image:
  placement: 3
  caption: 'Image credit: [**John Moeses Bauan**](https://unsplash.com/photos/OGZtQF8iC0g)'
---

The methods used to determine when we have a problem have changed over the years.

Alerting a person to a spike in CPU usage isn't as valuable these days. Especially those in the process of adopting the cloud. Instead, we want to know when our customer is experiencing a problem while using our system.

The problems will vary but the methods used to determine when a human needs to get involved have evolved.

By monitoring systems in a way that matches the customer's perspective we can see when they experience a problem rather than we *think* we experienced a problem.

If the customer is experiencing an issue, that's far more important to the business than any spike in CPU usage.

In today's connected world, no matter how complex or simple a system appears to be there is much more that goes in to what a user experiences.

It's entirely possible that all systems appear healthy and no alarms are going off when in reality users aren't able to complete a shopping purchase due to a third party payment processor. No amount of monitoring for memory or network performance would have tipped off engineers or leadership to this business impacting problem.

Every system is different and while there may be legitimate reasons to set up alerts for problems at the component level. However, by and large if we are planning to get engineers involved (especially outside of office hours) then we need to make sure the problem is real, it's impacting the business, and it requires human intervention immediately.

If an alert isn't actionable - meaning it requires a person or group of people to respond and investigate right away then it's not an incident.

If we can measure some minor details about when amd how we detect problems in the first place then we can look for opportunities to improve.

In conversations about what took place with the payment processor incident it is reasonable to ask "how could we have detected this sooner?".

"How could we have detected this ... at all?" may be a better question.

## Resources

[MS Learn: Improve Incident Response with Alerting in Azure](https://docs.microsoft.com/en-us/learn/modules/incident-response-with-alerting-on-azure/)

## Next steps

[Response Phase of an Incident](2020-03-04-Response.html)