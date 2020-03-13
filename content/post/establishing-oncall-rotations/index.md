---
title: Establishing On-call Rotations
date: 2020-03-05
image:
  placement: 3
profile: false
tags: ["rotations", "on-call", "coordination", "foundations"]
editable: true
---

People shouldn't have to be *on-call* for long periods of time. It's detrimental to their health and therefore the systems they create and look after.

In order to make sure people aren't expected to respond to problems 24-hours a day, indefinitely, we use rotations. Also referred to as scheduled shifts. That way people can take turns.

Being on-call requires a heavy cognitive task which then negatively impacts many aspects of a person's life. Shifts allow engineers to take “on-call” responsibility for their own specific recurring rotation and share the load in a way that keeps the human element a priority.

Site Reliability Engineering is an engineering discipline devoted to helping an organization **sustainably** achieve the appropriate level of reliability in their systems, services, and products. Long periods of on-call responsibilities is **not** sustainable.

When creating shifts there are a number of common approaches.

## 24 x 7

The majority of rotations used by teams are known as 27 x 7 shifts where engineers will be “on-call” for several days in a row. However, most “Elite/High performers” would agree that rotations longer than 3 or 4 days are detrimental to the overall health of engineering staff and therefore the entire system.  

## Follow the Sun

Follow the sun shifts are nice for distributed teams. These allow for engineers to schedule their “on-call” shifts only during their normal working office hours. As they end their day and go home, engineers in a different time zone can take over.

And of course, there are many ways to customize shifts, especially for weekends when engineers need more flexibility. Engineers should be able to hand off the role to someone when personal conflicts arise.

Once roles, rosters, and rotations have been determined and put in place, we can now focus our attion on methods of [Tracking Incident Details](/post/tracking-incident-details/)
