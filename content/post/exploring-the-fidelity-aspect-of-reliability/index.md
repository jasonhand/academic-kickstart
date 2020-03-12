---
title: Exploring the Fidelity Aspect of Reliability
date: 2020-03-05
profile: false
image:
  placement: 3
tags: ["reliability", "fidelity"]
editable: true
---

Fidelity pertains to the ability of your service to continue to provide a reduced or degraded experience when something goes wrong.

For example, if different parts of the home page on your website are provided by different microservices, and one of those microservices goes down, ideally you can still serve the home page with only that section missing or replaced with some static content.

Fidelity, then, is the measure of how often the page served that degraded or partial experience in comparison to serving the full page as intended with full fidelity.

It's common to architect systems in these graceful degradated states.

However, this means we need to pay attention to just how often and for what duration those degradations are taking place. Users will appreciate the resilient design but lose support if something is always broken from their perspective.

The next aspect of reliability applies to users who need real time information, updates, and access to take action on something.

[Exploring the Freshness Aspect of Reliability](/post/exploring-the-freshness-aspect-of-reliability/)