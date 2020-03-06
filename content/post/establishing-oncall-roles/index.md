---
title: Establishing On-call Roles
date: 2020-03-05
image:
  placement: 3
profile: false
tags: ["role", "on-call"]
---

Creating a repeatable response plan means establishing who does what when something goes wrong. We don't want there to be any question around who is supposed to be doing what.

Because of this, it is important to establish roles and the associated expectations. This isn't a separation of duties exercise. In fact, we want to encourage less of that. It is however, a way of establishing better coordination and communication. It prevents people from stepping on each others toes while enabling cross-collaboration amongst not only on-call rosters, but an entire organization.

**Primary Responder:** The first role we need to talk about is the “Primary Responder” – the Primary “On-call” engineer. 

This person is expected to acknowledge their awareness of an incident once the alert has been received.

**Secondary Responder:** Then we have the secondary responder – who is there as back up -Another engineer who can step in if the primary responder is unavailable or unreachable. Or if they just need another pair of eyes.

**Incident Commander:** Another key role to identify, in many cases, is the incident commander. An incident commander can be extremely helpful when you have got a large-scale outage that effects a lot of different components or requires coordination across many teams and different systems. They are great for making sure that engineers stay focused and they are working on their own remediation efforts... Ensuring people are not stepping on each other or undoing each other's work.  It is good to have a central person who can track what is going on and who is doing what.  

**Communication Coordinator:** The Communication Coordinator is meant to be the person working in conjunction with the incident commander to share more information beyond those who are in the firefight actively working to recover from the incident itself. That could be customers. It could be the sales and marketing teams. Maybe your customer support. There are many people within an organization who need to be made aware of what’s taking place and the status around how things are progressing. It's always good to put someone in charge of managing that communication and making sure that other stakeholders are aware of what is happening and what’s being done.

**Scribe:** The scribe’s role is to document the conversation in as much detail as possible. Teams commonly use phone bridges, conference calls, or video chat to get everyone together and try to understand what is going on, which can certainly help create space for the conversation. However, it is difficult for us to go through and understand in detail what the engineers were saying and doing unless it is transcribed. As a result, a scribe is that person who can help us document as much as possible to review later. What were people saying, doing, feeling, and even experiencing?  It is all data to be analyzed – but only if we capture it.

**Subject Matter Experts:** It’s quite common within on-call rosters to identify subject matter experts, so that early responders know who to escalate too quickly. These people should not be on call all the time, of course, but we do want to be able to identify who is our database expert. Who is our front-end expert? Who are the people that we can reach out to if our primary and secondary responders are not able to diagnose and resolve the issue themselves?

Let's take a closer look at each of these roles to better understand their place within our incident response efforts.

## Resources

[MS Learn: Improve Incident Response with Alerting in Azure](https://docs.microsoft.com/en-us/learn/modules/incident-response-with-alerting-on-azure/)

## Next steps

[The Primary Responder](/post/primary-responder/)