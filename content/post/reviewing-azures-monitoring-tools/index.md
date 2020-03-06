---
title: Reviewing Azure's Monitoring Tools
date: 2020-03-05
image:
  placement: 3
profile: false
tags: ["monitoring", "incident", "tools", "azure"]
editable: true
---

Azure Monitor includes a number of features and tools you can use to monitor and
measure reliability, using data from many different sources.

This article’s focus is to help you keep your “eyes on the prize” – the goal of
improving reliability in your organization. You should now understand what
reliability is and why it’s important. You know that operational awareness is an
essential precursor to monitoring for reliability, and that you need to
establish a baseline of “normal” behavior as a first step.

Now you’ll look at the practical question of how to go about doing that. As with
all complex tasks, the right tools can help you get the job done more quickly
and easily. In this unit, you’ll get a quick introduction to Azure Monitor,
Application Insights, and Log Analytics.

## Azure Monitor

Azure Monitor is a comprehensive platform for monitoring Azure resources to gain
insights into your applications, infrastructure, and network. In this module,
the focus will be on the Azure Monitor tools that you can use to monitor and
measure reliability.

A look at Azure Monitor starts with the data that comes into the system. Azure
Monitor takes in data from a number of different sources. These include:

-   Data from applications

-   Data from the various operating systems running in Azure

-   Information fed from Azure resources, subscriptions, and tenants

-   Custom data of any sort and from any source

There are many things we can do with that information: analyze it, visualize it,
integrate it, and respond to it when things go wrong.

## Data types

The data that comes into Azure Monitor can be divided into two types:

-   **Metrics:** small numerical pieces of information from counters, gauges,
    and so forth that are collected on a regular basis

-   **Log data:** information gathered from many different logs such as Windows
    event logs, Linux syslog, agents running on virtual machines, custom logs,
    telemetry from Application Insights, and more.

In this module, we will be focusing primarily on log data.

You can create, import, and export dashboards, using JSON files, to help you
better visualize the data and provide you with operational awareness about all
aspects of your Azure subscription, including reliability information. You can
also set access controls on the dashboards and share them with others.