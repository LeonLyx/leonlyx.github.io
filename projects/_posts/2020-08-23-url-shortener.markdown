---
layout: post
title: "URL Shortener"
date: 2020-08-23 00:00:00 +0800
author: Lin Yixiang, Leon
---

#### Reference
1. [URL Shortener Repository](https://github.com/LeonLyx/URL-Shortener)
<br/><br/>

#### Description
The objective of this web service is to generate a shortened version
of a given URL. The intent behind this project was to explore different
alternatives to better structure a nodeJS project, apply design principles 
and practice some clean code strategies.

Keys are pre-populated into the database to prevent the occurrence of the 
*Birthday Paradox*. Even though this feature is completed, further tuning on
the performance can be done. A cache can be included to store recently visited
URLs. If there is no cache, unnecessary overhead will be incurred when constantly
querying the database.