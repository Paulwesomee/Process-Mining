# Process-Mining Introduction
A repository to update about learning notes and reports, codes and projects about Service substitution based on process mining.
## What is Process mining?
Process mining can be seen as an analytic way bridging data analysis (data mining, ML, BI) and process model analysis (BPMN, etc. ) </br>
Process mining aims to offer optimaztion just like data mining but with proces, using **event log** to re-generate the business process that really happened and to gain insight from those generated processes.

## Play-in, Play-out and Replay</br>
**Replay**:   we start from both a process model and a collection of observed behavior, e.g. traces, and compare these.</br>
**Play-in**:  we start from event data and generate a process model, e.g. a Petri net.</br>
**Play-out**: we start from a process model and generate behavior, e.g. traces.

## A quick example 
To demostrate the flow of process mining, here we use an simple example:
First we have an event log:
```
A B C D
A C B D
A E D
```
Before using PM software or algorithm to analyse the event log, we could just judge by ourselve to have an understanding of what happened in the process flow. 
Clearly, the flow of this event **start with event A** and **end with event D**, while B\C\E are optional whether to show up, it seems that B and C aren't supposed to be done without one other in any sequence but we don't have enough sample size to find out. 
In conclusion we can form a shabby BPM as below:</br>
```
              ->B->C-|
Start -> A -->->C->B-|->D->End
              ->E----|
```
Alternatively, we could use some analyzing tools such as open source library of python, R , etc. to automatically generate the whole process:
![Pic1](https://github.com/Paulwesomee/Process-Mining/blob/main/Quick%20Sample/exercise1.png)	</br>
Generated using [PyProM](https://github.com/harrywang/pyprom), a lightweight Process Mining library of Python.


# Weekly lab report
This section is for the weekly report as a lab intern focusing on process mining. 

## Week ①  5.9-5.13
Following the [online courses of Eindhoven University of Technology](https://www.coursera.org/learn/process-mining), I have a comprehensive grasp of what process mining is and what it is capable of. </br>
1. Create this repository to record the learning and researching process </br>
2. Complete the first week's courses on coursera</br>
 - The introduction of process mining</br>
 - Some review about data analysis including Decision trees, Associate rule learning, clustering, etc. </br>
3. Finish the introduction of this repository about process mining</br>

##Week ② 5.16-5.19
1. Still following the course Process Mining to get a grasp of how we can perform process mining operations.</br>
2. Thesis reading- Behavioural service substitution</br>
2.1 Trying to understand the goal of service substitution </br>
2.2 Understand the new concept brought up - BPEL, Petri Net and Open Net

