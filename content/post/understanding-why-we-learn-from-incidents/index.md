---
title: Understanding Why We Learn From Incidents
date: 2020-03-05
image:
  placement: 3
profile: false
tags: ["analysis", "communication", "collaboration", "learning", "incident"]
editable: true
---

Incident response doesn’t stop when the incident is over. They say those who
don’t study history are doomed to repeat it. Likewise, those who don’t study,
analyze, and learn from the incidents they resolved are doomed to keep repeating
the process, as well.

Your most important means of learning from incidents is the post-incident
review.

When an incident occurs, your first reaction probably isn’t, “Hurray – a
learning opportunity!” Your immediate priority is figuring out what went wrong
and fixing it as quickly as possible, to reduce the impact on your customers and
end users – as it should be.

However, once the incident has been resolved, it’s important to follow up and
benefit from the discovery of whatever mistakes or circumstances led to the
failure. Doing so will help you prevent the same thing from happening again and
will also help you understand what tactics do and don’t work best when
responding to any kind of incident in the future.

The post-incident review is part of the analysis phase of the incident response
lifecycle. Not all post-incident reviews are created equal. There are different
ways to approach the process, and too much focus on certain aspects of the
problem or framing questions in the wrong way can reduce the value of the
review.

In this unit, you’ll start thinking about not only why but also how you can best
learn from incidents, and we’ll expand on the “how” in subsequent units.

## Complex systems fail

You must “learn to learn” from failure not in case your systems fail, but
because it’s a certainty that your systems *will* fail.

In the IT world, the majority of systems we work with today – especially in a
cloud environment – are complex. They’re composed of many interconnecting parts
that have to work together, and the behavior of the overall system comes from
the interaction of those parts, as much as from the individual parts themselves.

*Reliability* is the thread that runs throughout this learning path, but complex
systems are never one hundred percent reliable. Such systems behave in
interesting and counterintuitive ways. The complexity of these systems means
there are inevitably minor flaws within them, and it is difficult or impossible
to predict how minor flaws can join together to produce a significant incident.

For a more in-depth discussion of this topic, a good resource is the paper
titled *How Complex Systems Fail* by Dr. Richard I. Cook with the Cognitive
Technologies Laboratory at the University of Chicago. His “short treatise on the
nature of failure” explains the causative factors that are common to the
failures of complex systems of all types, in all fields.

[How Complex Systems
Fail](https://web.mit.edu/2.75/resources/random/How%20Complex%20Systems%20Fail.pdf)

Some of his key points are particularly relevant to the incident analysis and
post-incident review process:

-   **Complex systems contain changing mixtures of failure latent within them.**
    It is impossible for your systems to run without multiple flaws being
    present. The failures change constantly because of changing technology, work
    organization, and efforts to eradicate failure. Your system is never
    functioning perfectly.

-   **Complex systems run in degraded mode.** Complex systems are always running
    as “broken” systems. They keep “working” in that state because they contain
    many redundancies, and people can keep them functioning despite the presence
    of many flaws. System operations are dynamic, with components continually
    failing and being replaced.

-   **Catastrophe is always just around the corner.** The complexity of these
    systems means major system failures are – in the long term – unavoidable.
    Complex systems always possess the potential for catastrophic failure, and
    it can happen at any time. It is impossible to eliminate this potential
    because it’s part of the inherent nature of the system.

## Prevention and preparation

You’ve probably heard all your life the adage, attributed to Benjamin Franklin,
that “an ounce of prevention is worth a pound of cure.” The accepted meaning is
that it’s better to keep a problem from happening than to fix it after it’s
happened.

In your efforts to achieve a high level of reliability for your systems and
services, you should do everything possible to prevent incidents from occurring.
However, due to the complexity of those systems, as explained above, prevention
isn’t always possible.

Thus, you must take a two-pronged approach to failure: prevention on the one
hand, and when that isn’t possible, preparation to respond – quickly and
effectively. These two are interlinked.

Here’s an example of why it’s essential to do both: Sometimes an organization
will deploy an automated system. It works well. In fact, it works almost too
well – because people may take for granted that it will always work. They don’t
make proper preparation for the day that it doesn’t work. When that day comes –
as it inevitably will, sooner or later – and the system fails, it fails
spectacularly, and it’s much harder for operators to understand what went wrong.

The systems you work on are made up of more than the technology. In fact, you
don’t work “on” or “with” a system; you work *in* the system. You are part of
the system. Complex systems include both technical components (hardware,
software) and human components (people – and their personalities, training, and
knowledge).

How the humans respond when things go wrong is as important as preventing things
from going wrong in the first place. We learn from failure to respond faster and
better.

[Defining the Post-incident Review](/post/defining-the-post-incident-review/)