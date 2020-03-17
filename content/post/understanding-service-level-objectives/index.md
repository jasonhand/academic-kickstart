---
title: Understanding Service Level Objectives
date: 2020-03-05
profile: false
image:
  placement: 3
tags: ["measurements", "reliability", "slo", "service"]
editable: true
---

Now you know how to measure reliability using SLIs, but the ratios and
percentages that you’ve calculated only get you halfway toward fulfilling the
goal of site reliability engineering. You can now say the web server in our
example is 50% reliable, but is that the *appropriate level of reliability* as
discussed in our definition of SRE?

It's also useful to know the period of time to which that reliability level
applied. For how long was that 50% success rate maintained?

To answer these questions, you need to look at Service Level Objectives. SLOs
are statements of the objective you have from a reliability standpoint, based on
customer expectations. The basic recipe for creating an SLO consists of these
ingredients:

-   **The “thing” you’re going to measure –** number of requests, storage
    checks, operations; *what* you’re measuring.

-   **The desired proportion** – for example, “successful 50% of the time,” “can
    read 99.9% of the time,” “return in 10ms 90% of the time.”

-   **The time** – what timeframe are you measuring: the last 10 minutes, during
    the last quarter, in the previous 30 days, etc.?

    Putting these components together and including the important “where”
    information, a sample SLO might look like this:

    “90% of HTTP requests as reported by the load balancer succeeded in the last
    30 day window.”

[Building Service Level Objectives with Log Analytics](/post/building-service-level-objectives-with-log-analytics/)