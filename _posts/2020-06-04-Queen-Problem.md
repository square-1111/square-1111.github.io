---
layout: post
title: "Day 025, N-Queen Problem "
comments: true
description: ""
keywords: "dummy content"
---


Chess is a game of multi facets and has lots of mysteries with each piece. One piece in particular, assumed to be most powerful right after the king, the queen has made up a puzzle, the N-queens problem —  try to place N queens on a N\\(\times\\)N chessboard so that none of the queens attack each other.

Initially devised for the 8\\(\times\\)8 chess, that is to place queens such that none attack each other. The problem to find all the solutions to the 8-Queen problem is computationally expensive as there are <sub>64</sub>C<sub>8</sub> (= 4,42,61,65,368) possibilities out of which there are only 92 solutions. Is there a solution better than brute force? Given the constraints of Queens' move we can narrow down the possibilities. If we consider the straight movement of the queen we can narrow down the number to 8<sup>8</sup> (= 1,67,77,216) which can be further punched down to 8! =(40,320) by permuting the diagonal move of the queen. Out of the 92 solutions mentioned, if we do not consider symmetry operation of reflection and rotation then we are left with only 12 solutions. But as N goes up the value of N! goes up and causes trouble of computability.

While this time complexity can be optimized by using backtracking algorithms. Backtracking is a recursive process where the queen is placed on the edge and ideally saves the possible attacks. Then another queen is placed at a safe position and the process is repeated. However, if the N queens cannot be placed at safe positions then the algorithm backtracks and then try another safe position. This takes around 2<sup>N</sup> steps in the worst case which is 100 times faster than brute-force algorithm. 

We can still speed up the algorithm on the cost of storage. Known as Branch and Bound, this algorithm is similar to backtracking (described in previous paragraph) but keeps a track of the state of the board to prevent any unnecessary recursion. There are numerous other algorithms, some more efficient, others less but none of the algorithms have helped to cross the barrier to place 26 safe queens on 26\\(\times\\)26 chessboards. 

Moreso, as the size of the board increases the number of solutions to place the queens increases exponentially. Funnily,  for 5\\(\times\\)5 boards there are 10 distinct solutions and for 6\\(\times\\)6 boards the number of solutions drops to 4. There is no formula to calculate the number of solutions nor can we figure out the asymptotic limit. 

Similar to the N-queen problem, several other puzzles emerge from chess board like knights' tours. I sometimes wonder if we can ever explore all the possible states of a chess board and come up with new puzzles, who knows. 


