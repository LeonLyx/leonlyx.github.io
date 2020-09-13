---
layout: post
title: "Bus Arrival API"
date: 2020-08-24 00:00:00 +0800
author: Lin Yixiang, Leon
---

#### Reference
1. [Bus Arrival Repository](https://github.com/LeonLyx/sg-bus-api)
<br/><br/>

#### Description
Currently, there are public APIs available for [Bus Arrival](https://www.mytransport.sg/content/mytransport/home/dataMall/dynamic-data.html) 
in Singapore. The objective of this project is to create a wrapper that
encapsulates the internal design of the **Bus Arrival API**. Instead of
reinventing the wheel, developers can leverage upon this wrapper and 
concentrate on their business logic.

Personally, I am intending to use this Go wrapper to explore **R-Trees** and
understand how spatial queries are optimized. For instance, a typical
query can be, *"What bus stops are within 200m of my current location"*. At
present, I am still maintaining this project.
