---
layout: project
type: project
image: img/MastermindSquare.jpg
title: "Mastermind"
date: 2022
published: true
labels:
  - Java
  - Algorithms
  - Game Design
summary: "Built a game AI which breaks user generated code sequences"
---

<img class="img-fluid" src="../img/Mastermind.png">

<hr>

I started this project while I was taking a course on algorithms. In class we were given many different problems to solve as efficiently as possible using the data structures and algorithms we were learning about. Some of these puzzles reminded me of a board game I used to play with my Dad called Mastermind. In this game one player, the code maker, would create a code sequence of a specific length out of colored pieces. The second player, the code breaker, tries to guess the sequence within a number of tries. After each guess the code maker must reveal how many elements of the code have been guessed correctly (right color and correct spot) and how many are partially correct (right color but wrong spot).

I wanted to make a single player version of this game with multiple difficulty levels which would correspond to the efficiency of the algorithm used to solve the code. I started by designing the basic mechanics of the game using a text based interface. Designing the mode where the player was the code breaker was relatively easy. All I needed to do was display previous guesses and the feedback on correct and partially correct elements. The fun part was implementing the algorithms for the computer to use as the code breaker.

The easiest difficulty was using an inefficient algorithm. It would try to brute force the code by guessing random combinations. Although this approach is guaranteed to eventually find the right solution, it was very inefficient in terms of turns taken. The medium difficulty improved the efficiency by utilizing the feedback given to eliminate guesses. It would guess all one color, to determine how many elements of the code it comprised. It would then try to find the correct positions for each color. This behaves the most similarly to how I played the game with my Dad. 

The hardest difficulty utilized Kunth’s algorithm. The algorithm starts with a list of all possible codes. Before each guess, the algorithm determines which guess will maximize information gained and therefore minimize the number of possible guesses on the next turn. This is less resource efficient than other algorithms, requiring more memory and processing time. This is because the algorithm simulates the possibilities of each possible guess before it is made. It does however solve the code within a few guesses. For a four digit code with six possible colors, it usually solved the code within 4-5 guesses.

This project was a fun way for me to practice my algorithm skills. It allowed me to revisit a childhood game using my newly honed computer science techniques. It taught me that oftentimes, the most natural human approach to solving a problem is suboptimal due to the limitations of our brain. It would take an hour and dozens of pages of paper to play a game of Mastermind using Kunth’s algorithm by hand. However, we can use computers to overcome our brain’s deficiencies. 
