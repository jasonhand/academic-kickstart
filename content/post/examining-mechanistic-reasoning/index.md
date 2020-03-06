---
title: Examining Mechanistic Reasoning
date: 2020-03-05
image:
  placement: 3
profile: false
tags: ["incidents", "human", "analysis"]
editable: true
---

*Mechanistic reasoning* refers to the concept that a particular outcome can be
inferred from intervention. It’s sometimes called the *meddling kids syndrome*
based on the premise that “Our system would have worked fine … if it hadn’t been
for those meddling kids.”

When you use mechanistic reasoning in your post-incident review, you build your
conclusions on the fallacy that the systems you work with and within are
basically working correctly, and if only those “meddling kids” hadn’t done
whatever they did, the failure would not have occurred.

However, that’s not how systems work.

To illustrate this point, imagine the following scenario: You work on a
production service. Now you’re told that you are not allowed to touch or do
anything to that service. Everything outside your team continues as before –
customers continue to use the service, external dependencies continue to change,
the Internet functions normally.

But you can’t make any changes to the code or configuration. No deployments, no
control plane operations, nothing.

Do you think your service would still be running as expected after a day? After
a week? After a month? After a year? How long could you realistically expect
your service to keep running without human intervention?

*Human adaptive capacity is necessary to keep our systems up and running*.

The only reason your systems are up and running in the first place is because of
the actions of humans in the control loop. It’s only through human action
and ability to adapt to changing circumstances that the system continues to
work.

Therefore, it’s erroneous to conclude the system was “basically working…
if it hadn’t been for those meddling kids.” In fact, the reliability of your
service is not independent of the humans who work on it. Instead, it’s a direct
result of the work that the humans do on it every day.

The problem with mechanistic reasoning is that it leads you down a path where
you believe that finding the faulty human is equivalent to finding the problem.
However, that same faulty human has been improvising and adapting to keep the
system running for weeks and months.

[Examining Normative Language](/post/examining-normative-language/)