---
title: Creating an On-call Roster Using Azure Table Storage
date: 2020-03-13
profile: false
image:
  placement: 3
tags: ["on-call", "roster", "azure", "table storage"]
editable: true
---

On-call rosters allow teams to identify who is responsible to acknowledge and address incidents as they occur.

They are made up of the names and contact information of everyone expected to take part in the response and remediation of service disruptions.

|Name   |Email   |Service   |On-call   |
|---|---|---|---|
|Jason Hand   |jason@xyz.com   |API   |Yes   |
|Chris Smith   |chris@xyz.com   |API   |No   |
|Lauren Jones   |lauren@xyz.com   |Mobile   |Yes   |
|Ryan Boggs   |ryan@xyz.com   |Database   |Yes   |

Depending on the make up of your teams and services, on-call rosters can remain quite simple or become extremely complex.

One simple way of creating an on-call roster to look up and contact individuals in response to a service disruption is with a basic storage table in Azure.


[Establishing On-call Rotations](/post/establishing-oncall-rotations/)