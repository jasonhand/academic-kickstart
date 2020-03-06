---
title: Response Phase of an Incident
date: 2020-03-05
image:
  placement: 3
profile: false
tags: ["phase", "incident"]
editable: true
---

Once our detection efforts have been configured to send actionable alerts to the people who build the systems, we need to make sure they are sending those alerts to the *right* people.

## Right People

How do you know who the right people are? In most cases it is situational. A few things that can be done to help establish some formatlity and standard around responding to incidents is through the use of roles, rosters, and rotations. We'll go more in depth on what each of those are soon.

## Tooling

The right person for the job needs the right tools for the job. If someone is responding to an issue they need to get busy immediately. Making sure the right monitoring, communications, access, and documentation is provided is also important. People should be familiar with the tooling and know how and where to find additional resources to help diagnose, theorize, and triage.

### Diagnose

Everyone experiences problems. Sometimes routinely throughout the day in fact. When something doesn't go as expected or breaks entirely our impulse is to fix it. In order to do so we must first have a look at what's currently observable. What is the status? Who and what is impacted? What hints or clues are there? What information do we have to work with?  

What do we know *right now?*

### Theorize

Once information has been obtained, we begin to theorize next best steps.
What action can we take to minimize or stop the impact? What are the repurcussions of that action? Will something else go wrong? If we take one action, what result do we expect? In very brief moments we are creatively thinking through as many possible scenarios to restore service as we can. And then stack ranking them based on our own calculations on the probability of success.

## Triage

At some point we all need help. That could be access to an admin account, theories from subject matter experts, someone to amplify updates to a broader audience. Rarely are incidents viewed as a success if only a single person was involved.

Regardless of the size of your response team, by isolating it as a phase in the incident lifecycle, we can examine this section of the timeline for improvements on how we coordinate our response. If it took an excessive amount of time for the engineering team to correct the payment processor problem simply because it took too long to find the right person, with the right tool, and with the appropriate level of access then there are some clear opportunities for improvement right there.


## Resources

[MS Learn: Improve Incident Response with Alerting in Azure](https://docs.microsoft.com/en-us/learn/modules/incident-response-with-alerting-on-azure/)

[Remediation Phase of an Incident](/post/incident-remediation/)