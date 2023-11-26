# Ecosystem_Simulation
Theses programs simulate the interaction of different species over time.

The first programm is an advanced version of the Game of Life by John Horton Conway. It simulates the evolution of raccoons 
and foxes in a square field.

There are three differents animals in the simulation: two types of raccoon and the fox.
- the "normal" raccoon needs 2 or 3 friends to stay alive but dies with less than 2 or more than 3.
- the "alpha" raccoon only needs 1 or 2 friends but will die if alone or surrounded by 3 or more raccoons.
- the fox is the predator of the raccoons. The fox eats a nearby raccoon. It goes away if alone (it can't field itself)
  or is surrounded by 2 or more raccoons.
A normal raccoon is represented by a 1, a chad raccoon by a 2 and a fox by a 3.

A set of normal raccoons are randomly generated at the beginning. Later, a raccoon is born if an empty tile is 
surrounded by exactly 3 raccoons (the type of raccoon doesn't matter). It has a 1 in 20 chance of being a chad raccoon. 
A fox can randomly pop up (with a probability of 0.01) in the field in a tile close to one or no raccoon. 

Note : What makes the chad raccoon even rarer than at first glance is that it needs one of it's "parents" to die of 
overcrowding for it to survive the first day. If not, it would be surrounded by 3 other raccoons and die.

The "the ecosystem is stable" part could be improved but it's there only to prevent the code to repeat over and over just waiting 
for a fox to destroy the structure of raccoons.
