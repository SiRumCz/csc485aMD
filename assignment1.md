---
Author: Zhe(Kevin) Chen
Student number: V00819544
Date: Feb 03, 2018
---

<h1 align="center">Toyplot</h1>

## Table of Contents
1. [Assignment Overview](#assignment-overview)
2. [Introduction](#introduction)
3. [Quality Attribute Scenarios](#quality-attribute-scenarios)

## Assignment Overview
For target project, pick a quality attribute, create a quality attribute scenario, and document how the 
project source code realizes this scenario. Provide discussion on how the project can handle changes in 
this scenario in the future.

## Introduction
Toyplot[1] is an open-source python library from Sandia National Laboratories that develops beautiful 
interactive, animated plots that embrace the unique capabilities of electronic publishing and 
support reproducibility. It creates the possible data graphics out-of-the-box, maximizing data ink and 
minimizing chartjunk. It also comes with minimalist interface for engineers and scientists to explode.

The following content will be discussing one use case scenario and one growth scenario with their 
investigations based on one chosen quality attribute.


## Quality Attribute Scenarios
### Use Case Scenario
In the section I choose quality attribute Performance and create a simple scenario for Toyplot as it is 
basically a plotting toolkit, the most common use case is related to how it performs.

When a task calls a function in library to generate a normal sized plot, the whole process time must take 
less than 0.5 seconds from called to plot result.

| Aspect | Details |
|--------|---------|
|Scenario Name | Low latency on task performance |
|Business Goals | Efficient process speed to ensure user having low latency experience |
| Quality Attributes | Performance | 
| Stimulus | Need for generating a plot with 3 sinusoids from user |
| Stimulus Source | User and function in that module being called | 
| Response | Display the generated plot |
| Response Measure | < 0.5s process and render capability |

My response measure seems to be a reasonable guess since it is hard to get an estimation without getting 
hands on the toolkit and dig deeper into the source code.

### Use Case Scenario Investigation
In order to generate a basic three-sinusoids-plot as introduced in The Toyplot Tutorial[2] using the 
toolkit, it requires these steps to get the following result:

![alt text](https://raw.githubusercontent.com/SiRumCz/csc485aMD/master/a1_1.png)
