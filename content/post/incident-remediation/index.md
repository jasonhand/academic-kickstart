---
title: Incident Remediation
date: 2020-03-05
image:
  placement: 3
profile: false
tags: ["phase", "incident"]
---

The remediation phase is the blurriest of them all. A big reason is that sometimes there's no difference between what takes place during the response and an action intended to improve the situation (i.e. remediation step).

Much of incident response is just trial and error, quite honestly. We quickly think through what to do, we do it, we hope for quick feedback, we examine if things improved, and we iterate.

Because of this, measuring the remediation phase is a bit trickier.

What we are looking for is to determine the distinction between when we have *identified the fix* (or series of fixes) that will result in recovery of services and the end of the incident. What is the time between? Good or bad, it's data to potentially discuss and discover revelations.

It's not until the analysis phase that engineers can definitively determine the exact point along the incident timeline that everyone agrees the problem and solution were both understood. 

This underlines the importance of not only capturing the timeline of events, including conversations and actions taken but also analyzing it in retrospect with a diverse audience encouraged to ask questions. Questions that help radiate a broader and more informed knowledge base across an organization.

One reason for measuring this way is to set aside the time between definitively knowing what will restore service and when services were actually back.

Let's say the payment process thing from before was pretty easy to determine. It probably took less than 5 minutes to know it was something with the backend talking to an API and that after someone followed a specific series of steps everything would be fine.

However, the process to do this is not only complicated and requires administrative access, it's not well documented, and what is documented is extremely dated.

If this type of problem occurs again, we could shorten the total time of the incident, and therefore cost to the business, simply by making a few small adjustments.

These types of opportunities begin to surface when we can ask questions like, "how long does the backup script take?". "Was the documentation helpful?"

Just because you can figure out what the problem is in an acceptable amount of time, does not mean your system will recover as quickly as the business needs it to.

Once service is restored and things return to normal it's important to set aside time to reflect on what took place, discuss it openly, broadcast what has been learned, and prepare for the future.

This takes us to our next phase of the incident lifecycle - analysis.

## Resources

[MS Learn: Improve Incident Response with Alerting in Azure](https://docs.microsoft.com/en-us/learn/modules/incident-response-with-alerting-on-azure/)

[Analysis Phase of an Incident](/post/incident-analysis/)
