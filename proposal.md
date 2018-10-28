# X-Team 82 Project Proposal: Freshman PathFinder

See https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet#code for tips on using *Markdown* tags to format __.md__ files

## Goal

Work as a team to create a project proposal for your X-team to complete together.
The project does not have to be extremely difficult,
but there must be work to do for each member of your team.
You may reference figures using "See figure 1".  
Be sure to submit corresponding image files, i.e. figure1.png (or figure1.jpg) for each figure.

## Grading: To earn full credit, your team's proposal must include:

* (md) documentation: [this file] describing purpose and use of your program

* Description of a program that has:

  ** a main Java program class in a file named Main.java
  
  ** a custom data structure designed and built by your team
  
  ** comprehensive testing of individual units
  
 Caution: You are not being asked to implement this program, at least not yet. 
 We just want your group to make a proposal or pitch for your program.
 
 Tip: Your custom data structure can be composed of or extensions of data structures that you have learned and used in previous programming assignments.  We're looking for decisions about how to build a high-level data structure that will likely have lower-level components.

## Problem Description

Every freshman must take a lap of campus prior to the start of classes in order to ensure that he/she can easily get from class to class. But how can this be done efficiently so that one can get back to making new friends? Our program uses data from google maps to determine the most efficient path that a freshman (or forgetful upperclassman) can take to get a feel for the location of all of their classes.

## Questions to answer for Exercise #2

1. Name: Give your project proposal a name (and edit the top line of this file)
Freshman Pathfinder


2. Output: Describe the output your program will produce.

The program will output a list of the class locations with their Google Map locations, ordered in such a way as to minimize total time spent walking. Included also will be an estimate (pulled from Google Maps) of the total time required to complete the trip.

Example Output:

B102 Van Vleck https://www.google.com/maps/place/Van+Vleck+Hall/@43.0747707,-89.4045918,15z/data=!4m5!3m4!1s0x0:0x49bf687f6d3235d6!8m2!3d43.0747707!4d-89.4045918

CS 1366
https://www.google.com/maps/place/UW-Madison+Department+of+Computer+Sciences/@43.0714546,-89.4088143,17z/data=!3m1!4b1!4m5!3m4!1s0x8807accf4987c883:0x5c8312db7bc7df9!8m2!3d43.0714507!4d-89.4066203

Humanities 3650
https://www.google.com/maps/place/George+L+Mosse+Humanities+Building/@43.0741742,-89.4022384,17z/data=!3m1!4b1!4m5!3m4!1s0x8807accae420d1b3:0xff6a958a9f3b112f!8m2!3d43.0741703!4d-89.4000444

Social Sciences 5206
https://www.google.com/maps/place/William+H.+Sewell+Social+Sciences+Building,+1180+Observatory+Dr,+Madison,+WI+53706/@43.0765045,-89.4074916,17z/data=!3m1!4b1!4m5!3m4!1s0x8807acb62ed610c5:0xaeb4a15899906c15!8m2!3d43.0765006!4d-89.4052976

Total time to complete: ~30 minutes

Total time to complete: ~30 minutes

3. Input: Describe the data that is needed to solve your problem. Include an example format of the input data.

All the buildings the freshman want to visit

Example Input:
Humanities 3650
CS 1366
Social Sciences 5206

4. User Interface: Describe a user interface for your program.  Use text menus or a simple graphic user interface.



5. Types List: Break your solution idea down into units that you think can be implemented with a single class.



Name each interface or class and briefly describe its function or purpose.


## Edit and Submit this file and any figures referenced by this document.

