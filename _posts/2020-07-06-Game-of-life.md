---
layout: post
title: "Day 045, Game of Life"
comments: true
description: ""
keywords: "dummy content"
--- 

In 1970, John Conway published an eclectic paper about cellular automata — the game of life. It is a simulation that chooses how a complex thing like mind can come from a basic set of rules. This simulation consists of a grid, like a chessboard, extending infinitely in all directions. Each lid of the grid can either be lit up or dark.  

> **Cellular Automata** is a collection of colored cells in a grid like pattern to represent the state of that machine or program. It evolves over time according to the rules.

Game of Life is a zero player game, whose evolution depends on the initial stage of the game. Defined on 8 adjacent grid cells, the configuration of the next state depends on the configuration of the given cell and its corresponding neighbour cells. At each step in the time, following transitions can take place:

* If a cell is alive then it stays alive if it has either 2 or 3 live neighbours.
* If the cell is dead then it springs to life only in the case that it has 3 live neighbours.

The initial patterns constitute the seed of the system. This elementary cellular automata either blooms out or dies off. It is not necessary the structure becomes complex and intriguing nor is it necessary it must die off, there is a possibility that the structure oscillates and repeats itself every few moves. Block, beehive, loaf, boat — remain static and never change; blinker, toad, beacon oscillates, while glider and lightweight spaceship changes configuration over configuration and repeats the initial seed at different locations. 

<br>
<center><img src="/assets/images/conway_static.png" height="70%" width="70%">
</center>
<!-- <br>
<br> -->
<center><img src="/assets/images/conway_oscillate.png" height="70%" width="70%">
</center>
<!-- <br>
<br> -->
<center><img src="/assets/images/conway_repeat.png" height="70%" width="70%">
</center>
<br>


The behaviour of plants and animals can be better understood by these simple rules. Behaviour that seems intelligent, such as ant colonies might just be simple rules that we don’t understand yet. Traffic problems might be solved by analyzing them with the mathematical tool and breaking it down to fundamental. Computer viruses are also examples of cellular automata. Finding the pattern in these viruses might also be hidden in this life. Human diseases can be cured if we could better understand how cells live and die. Exploring the galaxies could be easier if the machines could be invented that could create a replica of themselves. Game of life helps in understanding all of this. 

Conway’s game of life is an existential proof that complex and unpredictable nature is possible due to a simple but recursive system.  

---

*<sup><sub>Images from [Chapter 7: The Nature of Code](https://natureofcode.com/book/chapter-7-cellular-automata/)</sub></sup>*

