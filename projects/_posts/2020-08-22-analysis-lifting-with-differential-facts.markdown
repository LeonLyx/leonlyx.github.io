---
layout: post
title: "Analysis Lifting with Differential Facts"
date: 2020-08-22 00:00:00 +0800
author: Lin Yixiang, Leon
---

#### Reference
1. [Overview of Analysis Lifting with Differential Facts](https://www.youtube.com/watch?v=7JhATQdfJTg)
2. [Project Demonstration](https://www.youtube.com/watch?v=QCZo56Hrn60&t=3s)
<br/><br/>

#### Description
In this project, there were 3 milestones to be met.

Firstly, I was expected to detect structual changes between two versions of any Java 
project. Firstly, each version's **Abstract Syntax Tree** (ASTs) is traversed using 
[Apache BCEL](https://commons.apache.org/proper/commons-bcel/) to obtain and extract 
the preliminary facts. Their respective call graphs will be constructed and the *difference* 
between two versions are then computed using a [Datalog-based program](https://souffle-lang.github.io/).

Following, I implemented **three types of analysis**, namely
**Def-Use, Constant Propagation and Reachability**. For Constant Propagation
and Reachability analysis, I have included two levels of granularity, 
which are **intra-procedural and inter-procedural**. All of the analysis were written 
on top of a Points-To analysis framework, [DOOP](http://doop.program-analysis.org/).

In the last phase, the objective was to apply [variability-aware techniques](https://arxiv.org/abs/1912.03854#:~:text=Variability%2Daware%20computing%20is%20the,Software%20Product%20Lines%20(SPLs).)
to perform program analysis. The purpose is to exploit the **commonality of program facts** across 
multiple software versions to speed up program analysis time.
