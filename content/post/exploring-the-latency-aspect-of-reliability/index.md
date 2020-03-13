---
title: Exploring the Latency Aspect of Reliability
date: 2020-03-05
profile: false
image:
  placement: 3
tags: ["reliability", "latency"]
editable: true
---

Latency refers to the amount of delay between a request and a response.

## Slow is the New Down

Today’s users have high expectations.

They demand fast performance and have little patience with a site or service that leaves them waiting. Reliability means the site is not only available, but available in a reasonable amount of time.

Especially for external customer interactions – for example, when a customer visits your company’s website – it is critical that the service respond as quickly as possible. A slow website can drive your customers to your competitors.

Azure is always [monitoring latency from points all around the world](https://docs.microsoft.com/en-us/azure/networking/azure-network-latency/?wt.mc_id=oncalllife-blog-jahand) to ensure speeds are within pre-defined limits.

![azure latency](https://docs.microsoft.com/en-us/azure/networking/media/azure-network-latency/azure-network-latency.png)

Let's say your service is available and fast, what else might users care about?

If your service returns the wrong thing, it’s not reliable in the eyes of your customers. 

It's supposed to work as advertised. If it returns the wrong results, calculates a bad value, or generally doesn't do what it's supposed to do "correctly", it's not relable to the user. Who wants to use a service that can't calculate for leap year, let alone manage your bank account?

[Take a look at the latency of Azure datacenters from your current location](http://azurespeedtest.azurewebsites.net/)

[![](latency-speed.gif)](http://azurespeedtest.azurewebsites.net/)

[Another one can be found here:](https://azurespeed.com/)

[![](latency-test.gif)](https://azurespeed.com/)

[Exploring the Correctness Aspect of Reliability](/post/exploring-the-correctness-aspect-of-reliability/)