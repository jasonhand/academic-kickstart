---
title: Understanding Service Level Indicators
date: 2020-03-05
profile: false
image:
  placement: 3
tags: ["measurements", "reliability", "sli", "service"]
editable: true
math: true
latex: true
---

[Site Reliability Engineering](https://docs.microsoft.com/en-us/azure/site-reliability-engineering/?wt.mc_id=oncalllife-blog-jahand) uses SLIs and SROs to measure the aspects of reliability that you learned about in Unit 2: availability, latency, throughput, coverage, correctness, fidelity, freshness, and durability, and whether you are
meeting expectations in each applicable area.

## What to measure

The first question to ask in relation to the aspect you want to measure is *what* to measure.

**Example \#1: Measure availability**

How would you determine the availability of a web server?

You can do this by measuring the number of HTTP calls the server received and the number to which it successfully responded. This ratio of successful calls to total calls gives you an understanding of the server’s reliability. Multiplying the ratio by 100 gives you a percentage.

$$
\ [\frac {success}{total}\] = ratio
$$ 

example

$$
\ [\frac {800}{1000}\] = .8
$$

For example, if the ratio is 0.8 and you multiply by 100, you can conclude that the web server has been available only 80% of the time.

or

$$
\ .8 * 100 = 80 percent
$$

**Example \#2: Measure latency**

To get an idea of the latency of the web service, you can measure the number of operations that were completed in fewer than 10 milliseconds against the number of total operations.

If, for example, dividing the first number by the second gives you a ratio of 0.8, and you multiply this by 100, your service has an 80% success rate by this measurement.

## Where to measure

To have a clear picture of your reliability based on SLIs, you need to know not only what was measured, but also *where* the measurement was taken.

For example, in measuring the availability of the web server above, you need to specify whether the number of calls was measured at the load balancer or at the server. Likewise, when measuring the latency of the web service, you should note that the number of operations was measured at the client.

Why is this so crucial? If the purpose is to create a feedback loop in your organization, in which you are able to have conversations about reliability using objective data, it is important for the people having these conversations to be using the same data.

To use a previous example, if you are trying to determine whether a web service is meeting expectations and one person looks at data collected at the server itself while another looks at data collected at the load balancer in front of that web server, you may be looking at radically different sets of numbers. The
information collected from the web server itself only reflects the traffic that actually reached that server. If there was an issue with the load balancer or the network and half the packets never reached the web server, the two people will have a very different picture of the situation, especially when it comes to
total number of requests.

This leads to the logical question: where is the best place to measure SLIs?

Unfortunately, there is not a universally “correct” answer. It’s a decision you must make with an understanding that there are tradeoffs either way.

The key thing to keep in mind is based on our “prime directive” of reliability measurement: *Reliability should be measured from the customer’s perspective.*
Thus, most of the time, you should measure at the point that most accurately reflects the customer’s experience.

{{< youtube Ds_7EKMS3N8 >}}
<br />

[Understanding Service Level Objectives (SLOs)](/post/understanding-service-level-objectives/)