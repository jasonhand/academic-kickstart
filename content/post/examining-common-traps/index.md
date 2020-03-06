---
title: Examining Common Traps
date: 2020-03-05
image:
  placement: 3
profile: false
tags: ["incidents", "human", "analysis"]
editable: true
---

As we delve into our post-incident review, we need to be on guard against some
human tendencies that can lead us to inaccurate or incomplete conclusions and
distract us from accomplishing the core purpose of the review: learning about
our systems so as to improve their reliability.

Now you have a roadmap help you get started on the post-incident review process,
but it would also be useful to know about some of the obstacles you might
encounter on this journey.

Learning from your own mistakes is something everyone should all do, but you
don’t always have to experience something first-hand to learn from it. Learning
from the mistakes of others, without criticizing or judging them, allows you to
benefit from those lessons without personally suffering the consequences.

In this unit, you’ll find out about some common traps that others have fallen
into during the post-incident review process and how to avoid them.

## Trap 1: Attribution to “human error”

(NOTE: It would be great to work the story about the B-17 accidents here. Insert
the video, or transcribe it into text here? We would need the photos to
illustrate it).

Humans make mistakes. However, *human error* is not a diagnosis; it’s a symptom.
When human error is deemed to be the reason for a failure, you may stop there
instead of further analyzing the incident to determine the *root cause –* which
is a deeper, systemic issue.

System design, organizational context, and personal context all affect when, how
and with what impact people make mistakes. *“*Human error*”* is a label that
causes you to quit investigating at precisely the moment when you’re about to
discover something interesting about your system.

The problem with the “human error” conclusion in investigations is that it
causes you to lose sight of the fact that what the humans did made sense to them
at the time. Mistakes, by definition, aren’t deliberate, so they didn’t intend
to make a mistake.

When we see or hear “human error”, it is a signal that we need to look deeper.
Root cause analysis is needed to identify the sequence of events that resulted
in the human error.

## Trap 2: Counterfactual reasoning

In the field of psychology, counterfactual thinking is a concept that’s
associated with the human tendency to invent possible alternatives to past
events – how things might have turned out differently.

*Counterfactual* means “contrary to facts,” and *counterfactual reasoning*
refers to telling a story about events that did not happen, in order to explain
the events that did. You can identify counterfactual statements by key phrases:

-   Could have

-   Should have

-   Would have

-   Failed to

-   Did not

-   If only

Some examples of counterfactual statements related to post-incident reviews:

“The monitoring system failed to detect the problem.”

“The engineer did not check the validity of the configuration before enacting
it.”

“This could have been picked up in the canary environment.”

The problem with this type of reasoning is that you’re talking about things that
didn’t happen instead of taking the time to understand how what did happen,
happened. You don’t learn anything from this speculation.

## Trap 3: Normative language

*Normativity* relates to the human tendency to designate some actions and
outcomes as desirable or good and other actions or outcomes as undesirable or
bad. A norm is a standard of correctness agreed upon by a society.

When you use normative language in a post-incident review, you judge the
decisions and actions of those responding to the incident with the benefit of
*hindsight*. This language implies that there was an obviously correct course of
action that the operator should have followed.

Normative language can usually be identified by adverbs such as “inadequately,”
“carelessly,” “hastily,” and so forth.

Normative thinking leads you to judge decisions based on their outcomes. This
isn’t logical because the outcome is the *only piece of information that was not
available* to those who made the decisions and judgments.

The problem with normative thinking is that you neglect to understand how the
actions of the operators made sense to them at the time.

## Trap 4: Mechanistic reasoning

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