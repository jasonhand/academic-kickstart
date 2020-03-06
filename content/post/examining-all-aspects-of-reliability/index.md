---
title: Examining All Aspects of Reliability
date: 2020-03-05
profile: false
image:
  placement: 3
tags: ["reliability"]
editable: true
---

There are eight important components that go into determining the reliability of
a system, service, application, or process. Consider whether and how each of
these is applicable in evaluating and improving the reliability of your systems
and services. Keep in mind, however, that reliability should always be measured
from the customer’s perspective, not the component perspective.

Raising your operational awareness and establishing a baseline of reliable
performance helps you to set expectations and recognize deviations from the
norm. After you establish a baseline, you can compare current performance to the
baseline statistics.

To create a baseline, you need to consider the many aspects of reliability that
combine to make up a person’s expectations. Some of these will apply to
particular applications and services but not to others. In all of these cases,
your goal is to understand and work with people’s expectations.

The important takeaway from this unit is this expanded idea of what reliability
means to your customers or internal users. Following are eight important aspects
of reliability to consider as you create your baseline.

## Availability

When people talk about reliability, they tend to start with availability. Is the
system "up" or is it "down"? Can others reach your website or your service? Can
they use the product when they expect to? This is important from the perspective
of both external customers and internal users who depend on your service. Thus,
availability is a good starting point for discussing reliability, but it’s only
one aspect.

## Latency

Latency refers to the amount of delay between a request and a response. You may
have heard the familiar catchphrase that “slow is the new down.” This refers to
today’s high customer expectations. People demand fast performance and they lose
patience with a site or service that leaves them waiting. Reliability means the
site is not only available, but available *right now* when the customer wants to
use it.

Especially for external customer interactions – for example, when a customer
visits your company’s website – it is critical that the service respond as
quickly as possible. A slow website can drive your customers to your
competitors, so latency is a reliability concern.

## Throughput

Throughput is a measure of the rate at which something is processed, or the
number of transactions that a website, application, or service successfully
handles over a specified period of time. This is particularly important when
running pipelines or batch processing systems. There are many factors that can
affect throughput. Monitoring throughput can help you pinpoint potential
problems that impact your users’ experience.

## Coverage

Coverage refers to how much of the data that you expected to process was
actually processed. Again, we come back to understanding expectations.
Reliability means getting the whole job done, every time.

## Correctness

An aspect of reliability that is often overlooked is “correctness,” or accuracy
of the results. Did the process that you ran on the data yield the correct or
expected result? This is an important factor to include in monitoring for
reliability. No matter how fast or “always available” your service or site is,
if it returns incorrect results, it’s not reliable in the eyes of your
customers. Monitoring for correctness of results is an important part of
monitoring for reliability.

## Fidelity

Fidelity in this context pertains to the ability of your service to continue to
provide a reduced or degraded experience when something goes wrong. For example,
if different parts of the home page on your website are provided by different
microservices, and one of those microservices goes down, ideally you can still
serve the home page with only that section missing or replaced with some static
content.

Fidelity, then, is the measure of how often the page served that degraded or
partial experience in comparison to serving the full page as intended with full
fidelity.

## Freshness

Freshness refers to how up-to-date the information is in situations where
timeliness matters to the customer. Examples would include sports scores or
election results, in which the data is constantly and quickly changing.
Freshness is not a factor for sites with static content that can remain the same
over time, but if your site serves time-sensitive information, customers will
expect that content to be kept current if they’re to consider the site reliable.

## Durability

Durability generally relates to longevity and resilience. It’s the ability to
remain functional over time. Durability is especially important in situations
such as storage systems where it is really crucial that a bit written to the
service can be read back out again later when desired.

## Reliability from the customer’s perspective

The eight components discussed in this unit all go together to make up the idea
of reliability. Not all of the factors will apply in every situation. When
considering these factors, the most important point to remember is that
reliability has to be measured from the customer’s perspective, not the
component perspective.

[Understanding Measurements of Reliability](/post/understanding-measurements-of-reliability/)