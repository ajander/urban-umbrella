---
layout: post
title: "Project Overview"
subtitle: "Bird Behavior App"
date: 2023-06-12
category: "Bird Behavior App"
---

<img src="./urban-umbrella/assets/finch_on_feeder.jpg" alt="finch on a bird feeder" width="200>

![finch on a bird feeder](/urban-umbrella/assets/finch_on_feeder.jpg)

### Goal
To measure the rate at which the birds in my backyard are eating from the bird feeder and to display the data in a web app. 

The amount of food eaten in a given time period will be measured by the change in the weight of the bird feeder during that period. 

### Questions

* What daily/seasonal trends exist in feeding rates?
* What other factors affect feeding rates, e.g., weather, type of food offered?
* Is it possible to detect when an individual bird lands and therefore count and possibly identify visitors?

## Hardware

The birdfeeder will hang from a load cell that will measure its weight. The load cell connects to a load cell amplifier, which connects to a WiFi microcontroller to send the data to the cloud.

## Software

Planned software components are:
* AWS for data ingestion, processing, and storage. Possible pipelines:
  * AWS IoT Core &rarr; S3
  * AWS IoT Core  &rarr; Kinesis  &rarr; S3 via Lambda
* Streamlit to visualize the data
