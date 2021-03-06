This is the code of a robot that clean a room. The robot will take the measures of the room. Walk over it and clean every tile that he passes on. He will keep track of the tiles he was on and that has been cleaned in order to minimize repeated movements. 

The robot follow this cleaning strategy:<br>
1- Check if the tile in front of you is clean<br>
2- if clean move your direction by 30 degrees<br>
3- repeat number 2 until you find a dirty tile<br>
4- if no dirty tiles are found and the whole surrounding is checked: move to a random tile<br>
5- repeat the earlier steps<br>
6- if the robot hits a wall, he will change the direction by 30 degrees until he finds a tile.<br>

I have tried different angels and from the results I got, 30 degrees gave the best results and the fastest cleaning.

The function ‘updatePositionAndClean’ in the robot class controls the movement strategy of the robot.

In each function is a short explanations of what the functions is expected to do.
Each step is also explained in the inline comments.

If you uncomment the ‘anim’ in the ‘runSimulation’ you will be able to see the robot moving in the room:

<img src='https://github.com/nos111/Cleaning-robot/blob/master/images/RobotMovementSimulation.jpg?raw=true'>


Functions to provide analytical data are provided:
<h2>-“showPlot1”  Produces a plot showing dependence of cleaning time on room size.</h2>
<img src='https://github.com/nos111/Cleaning-robot/blob/master/images/GraphTimeXRoomSize.jpg?raw=true'>

<h2>-“showPlot2’ Produces a plot showing dependence of cleaning time on number of robots.</h2>
<img src='https://github.com/nos111/Cleaning-robot/blob/master/images/GraphTimeVSRobotsNumber.jpg?raw=true'>


<h2>-“showPlot3” Produces a plot showing dependence of cleaning time on room shape.
</h2>
<img src="https://github.com/nos111/Cleaning-robot/blob/master/images/GraphTimeVSRoomSizeRatio.jpg?raw=true">

<h2>-“showPlot4” Produces a plot showing cleaning time vs. percentage cleaned, for
each of 1-5 robots.
</h2>
<img src="https://github.com/nos111/Cleaning-robot/blob/master/images/GraphTimeVSPercentageCleaned.png?raw=true">

<h2>-"showPlot5" Produces a plot comparing the two robot strategies.
</h2>
