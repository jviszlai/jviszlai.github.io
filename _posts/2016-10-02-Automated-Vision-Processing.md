---
layout: post
title: Automated Vision Processing
---

This project was an automated vision processing program meant to help quickly process and adjust the aim for shots during a robotics competition, [FIRST Stronghold](https://en.wikipedia.org/wiki/FIRST_Stronghold). The goal of the project was to effectively identify the best spot to shoot in order to score, be able to adjust the robot accordingly, and perform these tasks with little delay.

I worked with 2 other team members to develop all the code for the robot, including the robot Java code on the main processor and the vision processing code on a Raspberry Pi coprocessor, however, I mainly worked on the vision processing, so that's what I've included on this project page.

The program was written using Python along with the library, [OpenCV](http://opencv.org/). The purpose of the program was to identify a goal (in the case of the competition this was a hole in a tower) outlined in reflective tape, and relay instructions to the main processor on adjustments necessary to aim a shot properly.

The biggest challenge proved to be isolating the goal from random lights in the room that had similar color values, however, to solve this, the program isolates objects of the target color that also have the number of corners as the goal outline, which was 8, and then identifies the largest remaining object as the goal. This proved effective approximately 1 out of every 8 frames or so, due to the occasional false detection of a large light and the way the program approximates corners. To adjust for this, the program also finds the most frequently detected object out of every 5 frames and only sends adjustment data for that object.

<img src="/downloads/ControlAward.jpg" width="150" align="right">

This program proved extremely effective and took noticeably less time to process than other popular methods of teams from both that year and years past. Because of this, at our first competition of the season we were awarded the innovation in control award, given to a team for innovative ways of programming their robot.

The Python code for this project can be found on GitHub [here](https://github.com/jviszlai/OpenCV-FRC-Vision-Processing).

Below I've also included a cool gif of the robot running the program during competition.

<img src="/downloads/autoshot.gif">