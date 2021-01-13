# Starter project

This project has a Starter project - [https://scratch.mit.edu/projects/455279461/](https://scratch.mit.edu/projects/455279461/)

Log in to your Scratch account and Remix this project and save it to your account. You can rename it if you wish.

When you open the Starter project you’ll see the layout of a crossroads with two sets of traffic lights, which aren’t yet working.

If you click the green flag you’ll see cars start ‘driving’ from left to right & from bottom to top. You might see some near misses!



The task of this project is to add code to the traffic lights in order that the traffic is controlled. i.e. cars will queue when the lights are at red, will slow down when the lights are at amber and will only ‘go’ when the lights are at green, as illustrated in this screen capture.



## Contents of the Starter project

The starter project has some sprites with some pieces code already included:

### Backdrop and Sprites:

* a Stage Backdrop showing the green field and crossroads with white ‘stop’ lines
* a Car X sprite, which generates the cars moving horizontally; left to right
* a Car Y sprite, which generates the cars moving vertically; bottom to top
* a Lights X sprite, used to control the cars moving horizontally
* a Lights Y sprite, used to control the cars moving vertically
* a Start Button sprite, which will be used to turn the lights ‘on’, after they have been ‘installed’

### Code

* code on the **Stage** to initialise some variables and lists that are available to all sprites
* code on the **Car X** and **Car Y** sprites that:
  * generates multiple cars of differing colours using clones
  * controls the speed of the cars based on:
    * the current colour of the lights (off, red, red & amber, or green)
    * the distance from the white ‘stop’ line in front of the lights, and
    * the distance between the car itself and the car in front

### Costumes

Each light sprite (Lights X and Lights Y) has 5 costumes. The name of each costume shown in this table:

### ‘Lights X State’ and ‘Lights Y State’ global variables

The code for the movement of the cars relies on the values of variables that are available for all sprites:

* Lights X State variable showing the current state of the lights for the cars moving in the horizontal direction, and

* Lights Y State variable showing the current state of the lights for the cars moving in the vertical direction.

The possible values for the variables correspond to the names of the costumes. They are:
* red
* red&amber
* green
* amber
* off

The following steps show how to create the code needed to generate the correct settings for Lights X State and Lights Y State, which will in turn cause the traffic to be controlled.