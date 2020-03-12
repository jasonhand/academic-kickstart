---
title: Exploring the Availability Aspect of Reliability
date: 2020-03-05
profile: false
image:
  placement: 3
tags: ["reliability", "availability"]
editable: true
---

**Can people reach a website or service?**

This is typically the first thing people think of when talking about reliability. Can "the thing" be reached (and used) when expected?

This is important from the perspective of both external and internal users who depend on a service. Because of this, availability is a good place to start discussing reliability.

## Availability

If a service can't be reached at all then it is of no value to its intended user and in some cases detrimental. Availability lets us communicate whether or not our service is ready to go.

In terms of monitoring for availability, we could set alerts for low disk space of service. This could tip us off to an imminent problem that is known to impact the availability of a service.  

We could also examine logs that tell us in aggregate what the customer is experiencing when attempting to communicate with our service. Are they gaining access or receiving responses? Or are they seeing 404 and 501 error codes?

Answering those questions gives a more accurate picture of the availability of your service. Just because everything appears to be working, does not mean that is what your user is seeing.

You can't always do something about availability. The number of hops between a website and a person's mobile device is astounding. Failure could happen at any point between them.

The closer we can measure that experience from their perspective, the better off we'll be in measuring our availability.

The next aspect of reliability that often gets a lot of attention is latency. Despite your service being available, if it takes too long to communicate back and forth, there's no denying it is a bad experience for the user. In the high speed world, patience for slow services is nearly non-existent.

[Exploring the Latency Aspect of Reliability](/post/exploring-the-latency-aspect-of-reliability/)