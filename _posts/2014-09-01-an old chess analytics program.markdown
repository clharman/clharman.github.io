---
layout: post
title:  "An Old Chess Analytics Program"
date:   2014-08-16 00:00:00
categories: project update chess
---

During winter break 2013 I briefly ideated and worked on a project intended to help chess players improve their game.  The idea behind it is that chess competency is built on patterns -- "habits," if you will, either good or bad.  Computers, being very good at both recognizing patterns and playing chess, seem like a natural tool to aid in chess learning.  Of course, computers approach the game of chess in a very different way, i.e. they see decision trees and preset rules while a skilled human sees strengths and weaknesses.

So how can these different approaches be reconciled to each other?  As one might expect, it is impossible.  That is, until a chess engine is created that thinks like a human.  In the meantime, the easiest way to extract value from a computer's thoughts seems to be its scoring system.  When computers assess positions to choose moves they assign scores to each position in their analysis.  This score is often a good indicator of the balance of the game.  For example, if the score is +3.0, white has a comfortable advantage.  Maybe he is up three pawns (as the scoring system is usually in units of pawns).  If the score is -0.7, perhaps material is even but black has a very strong pawn center.

My first idea to utilize the computer's score was to look for blunders, defined as, basically, terrible moves.  Computers and humans see blunders in about the same way.  Give away a queen?  Lose 9 points and the game.  Pretty straight forward.

In order to implement a blunder check I first learned how to communicate with a chess engine.  Programming a chess engine is an extremely difficult problem and I was not about to attempt it, but open source engines exist and most communicate using a protocol called UCI.  Using the UCI protocol I was able to pass moves into the engine and receive numerous outputs including move branches and scores.  I ran into trouble when the scores I was reading did not reflect the situation on the board.  For example, I was using an archived online game of mine as a test in which I give away my queen on the last move.  However, the engine failed to adjust its score to reflect the obvious swing in material advantage.

At that point I ran out of time to work on the project, but I hope to resume and create something useful when I have time.  All coding is done in Python, some modules are used, and more information can be found on the [github repository](https://github.com/clharman/ChesStream).