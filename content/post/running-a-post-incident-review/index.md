---
title: Running a Post-incident Review
date: 2020-03-05
image:
  placement: 3
profile: false
tags: ["incident", "analysis"]
editable: true
---

There are different ways to conduct a useful post-incident review, but there are
some common practices that can make the process easier and more effective. If
you run a facilitated review meeting, keep your review and planning meetings
separate, ask better questions, and identify how things went right, you can
learn more and use what you learn to improve the reliability of your systems,
services, and processes.

Now you’re aware of some of the common pitfalls that can sabotage your
post-incident review, and you know what *not* to do. The next logical question
is “what should you do instead?”

In this unit, you’ll learn about four helpful practices that can make your
response team better and improve the post-incident analysis process.

## Practice 1: Run a facilitated post-incident review

You already know that a post-incident review is not a document or report, so it
follows that having one person write up a “postmortem” of what happened doesn’t
make for a helpful post-incident review. No matter how knowledgeable or how
deeply involved in the incident that person might be, not much will be learned
if everything comes from a single viewpoint.

Getting those who were involved in the incident together at the same time is the
first step. But there is something else you can do to increase the useful
learning that comes out of the review even more.

A *facilitator* is someone or something that makes an action or process easier.
To make the post-incident review process both easier and more effective, you
should plan to have a post-incident review meeting with a *neutral facilitator*
– someone who was not involved in the response to this incident.

Everyone will learn more if the facilitator cannot be seen to have any
preconceived ideas or a personal agenda in telling the story of the incident.

The exact format for the meeting will depend on your team, scheduling, and the
nature of the incident, but here are some more basic guidelines:

-   **Meetings, not marathons:** the meetings don’t have to be long. Generally,
    sixty to ninety minutes is the maximum length of time most people can fully
    concentrate and participate effectively, so limit the meeting to not more
    than an hour and a half.

-   **Pre**-**meeting prep:** to make better use of the meeting time, it can be
    helpful for the facilitator to prepare by conducting one-to-one interviews
    with some of the members of the response team to get an overview of the
    incident and ideas about which topics to talk about in the meeting.
    Individual interviews are also appropriate with certain personalities, when
    presenting in front of the room is a cause for discomfort.

-   **Not required for every incident**: this is a learning process, and you’re
    “learning to learn,” so start small. You don’t have to do this for every
    incident. You can pick and choose. You might want to start with smaller
    incidents or start with a review meeting only once per month.

The post-incident review meeting is an opportunity to find out what went wrong,
what was done right, and how failures can be handled better in the future. The
ultimate goal is to improve reliability.

## Practice 2: Ask better questions

You already know that language matters, and in the post-incident review, this
applies especially to the questions you ask. Objective questions will usually
elicit more useful answers.

*In particular, it’s better to ask people “how” or “what” instead of “why.”*

When people are asked to explain “why” they did something or “why” something
happened, it tends to put them on the defensive. Beginning a question with “why”
often comes across as a judgement, criticism, or accusation. It forces people to
justify their actions, and people don’t always know why they did something, or
why something happened as a result of their actions.

This doesn’t mean you can’t explore the reasons the incident occurred or the
reasoning a person used to decide what to do in response to it. It just means
you should pay attention to how you word those questions:

Don’t ask “why did you do that?” 

Instead, ask “*what factored into your decision to make that change?*”

Don’t ask “why wasn’t this caught in canary?”

Instead, ask “*how effective is canary at catching this sort of issue,
usually?*”

Remember that the post-incident review is about learning. Each participant in
the incident is likely to have had a slightly different view on events. You’ll
learn more if you ask questions that expose these multiple views and
interpretations.

Don’t get tunnel vision. Sometimes focusing too narrowly on the incident in
question will cause you to miss valuable information. You will often learn as
much by asking about how work “normally” happens as you will by asking about the
specific incident.

To learn more about how to ask better questions, check out this resource:

[The Etsy Debriefing Facilitation
Guide](https://extfiles.etsy.com/DebriefingFacilitationGuide.pdf)

## Practice 3: Ask how things went right

When you think about learning from failure, you may forget that even within a
major outage or other incident, in addition to the things that go wrong there
are also things that go right. Far from our view of incidents as one-offs or
products of extreme conditions, in most complex systems things go wrong for many
of the same reasons they go right.

It’s human nature to focus your questions on the negative side of the equation.
However, also asking about how things went right will provide you with insights
that you would not have gotten otherwise.

*Don’t just ask how the outage happened.*

*Ask how your team recovered the systems.*

You want to know what insights, tools, skills, and people helped in the recovery
effort. These are things you want to be able to reproduce, so this information
will be valuable in planning what to do going forward.

In this context, you want to ask how people came to know what they knew and on
what basis they made the decisions they made. Was there a critical moment when
someone shared a piece of information that helped unlock the puzzle of what was
happening? How did they know to do that? Where did the information come from?

Look for themes and patterns. Finally, as part of recognizing what went right,
ask *What do you know now that you didn’t know previously?* If learning resulted
from the incident and from the incident response and review processes, that’s
another thing that went right.

## Practice 4: Keep review and planning meetings separate

After you’ve resolved the immediate incident, you’re naturally going to want to
talk about repair items and future mitigation – and you should – but these
topics should *not* be a part of your post-incident review meeting. Your
post-incident review meeting has a purpose and allowing the discussion of repair
items into that meeting will distract from that purpose.

The best plan is to discuss repair items and planning issues in a separate
meeting a day or two after your post-incident review. You might want to do this
with a smaller group. Both of the meetings will be more productive as a result
of this separation.

It will help you keep the focus of the post-incident review where it belongs, on
what actually happened. In addition, allowing a day or two of “soak time” will
result in better “synthesis,” giving your subconscious time to work on the
issues. This will help you to identify the most “energy-efficient” repair items
– those that require minimum energy for maximum impact.

[Gathering Data for the Post-incident Review](/post/gathering-data-for-the-post-incident-review/)