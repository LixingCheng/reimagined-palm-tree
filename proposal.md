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

The program will output a list of the class locations with their Google Map locations, ordered in such a way as to minimize total time spent walking. Included also will be an estimate (pulled from Google Maps) of the total walking time required to complete the trip.

Example Output:

Starting from: Witte Hall

1) B102 Van Vleck https://www.google.com/maps/place/Van+Vleck+Hall/@43.0747707,-89.4045918,15z/data=!4m5!3m4!1s0x0:0x49bf687f6d3235d6!8m2!3d43.0747707!4d-89.4045918

2) CS 1366
https://www.google.com/maps/place/UW-Madison+Department+of+Computer+Sciences/@43.0714546,-89.4088143,17z/data=!3m1!4b1!4m5!3m4!1s0x8807accf4987c883:0x5c8312db7bc7df9!8m2!3d43.0714507!4d-89.4066203

3) Humanities 3650
https://www.google.com/maps/place/George+L+Mosse+Humanities+Building/@43.0741742,-89.4022384,17z/data=!3m1!4b1!4m5!3m4!1s0x8807accae420d1b3:0xff6a958a9f3b112f!8m2!3d43.0741703!4d-89.4000444

4) Social Sciences 5206
https://www.google.com/maps/place/William+H.+Sewell+Social+Sciences+Building,+1180+Observatory+Dr,+Madison,+WI+53706/@43.0765045,-89.4074916,17z/data=!3m1!4b1!4m5!3m4!1s0x8807acb62ed610c5:0xaeb4a15899906c15!8m2!3d43.0765006!4d-89.4052976

Total time to complete trip: ~30 minutes

3. Input: Describe the data that is needed to solve your problem. Include an example format of the input data.

- Starting Point: a single dorm hall
- Class locations: a list of the buildings the freshman wants to visit

Example Input:

Witte

Humanities 3650
CS 1366
Social Sciences 5206

4. User Interface: Describe a user interface for your program.  Use text menus or a simple graphic user interface.

The user will see a search bar/box that says "Start Typing", in this box the user will begin typing the dorm that they live in which will be their starting point. As they type, the program will begin suggesting results pulled from a pre-loaded list of dorm buildings. 

After selecting a dorm, the user will press a button to start adding buildings. Another search bar will appear and the user will start typing the first class location they wish to input. Similar to the dorm selection, as they type, the program will begin suggesting results pulled from a pre-loaded list of class buildings. Once a building is selected, the user will be able to use a small "add location" button to gain access to another search box in which they can add another class location. In this manner the user will enter in all of the campus buildings they wish to visit. Once the user is satisfied with their building list, they will press a "map" button at the bottom of the screen. 

On completion of the path calculation, the user will be shown an list of their inputed locations (ordered for walking-time minimization) with a google maps link next to each. From here they can click any of the links to be brought to their google maps app, in which they can obtain walking directions if necessary.


5. Types List: Break your solution idea down into units that you think can be implemented with a single class.

- Node class with the following fields/methods:
   - GPS Coordinates (Vector)
   - Building Name (String)
   - Identifier (int)
   - List of Out-edges (linked list of edge-objects, defined as inner class below)
   - Visited (boolean)
   - Constructor method
 
- Inner class defined within Node with the following fields, for use in out-edge list):
   - Pointer to other Node
   - Edge weight, calculated with google maps API, stored as Double.
 
- Graph class with the following methods/fields:
   - List of all nodes in graph (field)
   - Main method + supporting methods to carry out computation (Dijkstra's Algo. most likely)
   - Method to pull data from google maps (to determine edge weight)
   - Graph constructor




## Edit and Submit this file and any figures referenced by this document.

