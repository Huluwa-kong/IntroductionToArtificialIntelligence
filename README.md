# IntroductionToArtificialIntelligence
School of Computer Science The University of Adelaide 



## Assignment 3
1 Robot localisation (UG and PG)
Robot localization is the process of determining where a mobile robot is located con- cerning its environment. Robot localization provides an answer to the question: Where is the robot now? A reliable solution to the localization is one of the most fundamental competencies required by an autonomous robot as the knowledge of the robot’s own location is an essential precursor to making decisions about future actions.
In a typical robot localization scenario, a map of the environment is available and the robot is equipped with sensors that observe the environment as well as monitor its own motion. The localization problem then becomes one of estimating the robot’s position within the map using information gathered from these sensors. The following shows an example of a 2D map drawn using ASCII characters:

The character ‘X’ denotes an obstacle (the path cannot be traversed), while the character ‘0’ (Zero) represents a traversable positions. Any position within the map is indicated by the coordinates (k, j), where k is the row number (ordered top to bottom) and j is the column number (ordered left to right), starting from 1. For example, the top left position is (1, 1) and the bottom right is (4, 10).
A robot moves in the map and gathers information along the way. In this version, the robot has a single non-deterministic Move action and its sensors reports whether or not obstacles lay immediately to the north, south, east, and west. A sequence of

• The state variable Xt represents the location of the robot on the discrete grid; the domain of this variable is the set of traversable points illustrated as ‘0’ points in the map.
• Let NEIGHBORS(i) be the set of traversable points that are adjacent to and let N(i) be the size of that set. Then the transition model for the Move action is defined as follows, which means the robot has equal probability to move to each of its neighbours.

1.2 Deliverables
Write your robot localisation program in Python 3.6.9 in a file called viterbi.py. Your program must be able to run as follows:
$ python viterbi.py [input]


如果您需要任何关于此assignment的帮助，可以联系vx:codingtuto
