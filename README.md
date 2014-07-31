So many ideas, so little time ...

mogtools
========

Tools for multiplayer online games.
Similar to DirectPlay, but for non-Windows platforms.
http://msdn.microsoft.com/en-us/library/windows/desktop/bb153243%28v=vs.85%29.aspx

Features:
- lobby
- chat
- users and user groups
- client-server or peer-to-peer
- sessions
- easy to synchronize game entities
- TCP, UDP, HTTP, websockets


RAMM
====

Ranker and Match-Maker, based on bots. Purpose: try different MM and ranking algos, unit-testing, and load-testing

phase 1
- players are simulated by bots
- 100 bots with different skill level (some have the same skill level)
- the 2-player game is a 10-side dice roll: the highest roll wins (if tie, reroll)
- skilled bots have high dice-roll mean
- all bots have same stdev
- the simulation runs "days" (ie recompute ranks at the end of the day)
- one match per bot per day
- simple algos


phase 2 
- skill improves over the days
- different skill stdev
- ELO
- take into acount the scores (score of 10 to 1 vs score of 5 to 4)


phase 3
- fancy algos (gradient descent, gaussian density filtering, ...)



Ant Colony
====

Inspired by Rollings and Morris' book 2004 on game design.
The player interacts with a colony of ants by influencing the actions of some individuals 
or sending macro events (food, predator, rain). 
The player does NOT build the ant colony, but rather simply interacts with the simulation in interesting ways.

The colony starts with ~50 ants. 
The player gains new ways to interact with the colony when the population reaches thresholds.
For example, at 1k ants the player can start using a landslide, and at 100k an anteater.  

Neural networks and genetic algorithms?



Mandelrian
===

Mandelbrot Fractals of Mondrian, like http://kottke.org/11/02/fractal-mondrian



Raspberry Pi
====

http://www.raspberrypi.org/faqs



Game engine using Oryx sprites
====

http://forums.tigsource.com/index.php?topic=8834.0
http://forums.tigsource.com/index.php?topic=8970.0
http://forums.tigsource.com/index.php?topic=9147.0


FTL clone with ronin samurai instead of spaceship
====
http://www.ftlgame.com/
Replace fuel by food, sectors by provinces, beacons by villages, missile-launchers by bows, lasers by swords.


Abbey Manager: REST multiplayer management game using ncurses
====

- ncurses: See this list. http://www.use-strict.de/list-of-cool-ncurses-games.html and Curse of War https://www.youtube.com/watch?v=FZH4qbIxpx4
- REST would probably work well for multiplayer games like Drug Wars, Travian, or Football Manager: no real-time interactions, slow gameplay at the scale of hours or days, not seconds.
- theme: the abbey of The Name of the Rose. You are a 14th-century abbot, managing an abbey of 60 monks and 150 servants, with a library, infirmary, church, smithy, brewery, etc. Quotes from the book, p39-41: "it has more books than any other Christian library", "your abbey is theo nly light that Christianity can oppose to the thirty-six libraries of Baghdad", "many of the monks living in your midst come from other abbeys scattered all over the world. Some stay here a short time, to copy manuscripts to be found nowhere else, not without having brought you some manuscript or great rarity in exchange. Others stay here for a very long time because only here can they find the works that enlighten their research.", "Only the librarian knows where to find a book in the labyrinth of the library, which truths and falsehoods it contains, and who should or should not read it."



Shadow of the Colossus/Monster Hunter in 2D
===

Get a bounty for a monster, kill that monster, receive bounty reward, improve gear, get higher bounty, repeat.
Each monster has a particular behavior, eg a crab moves sideways and can only be attacked from behind.
Maybe the code from crowd-control could work for that.


Map generator
===

Like Diablo or roguelike games. Maps are made of at most 10 blocks of 50x50 cells. Each block can have up to 4 gates, eg a North gate is a hole from 24,0 to 25,0, and the rest of row 0 are walls. Each block must have at least one gate. Blocks can be hand-made or generated. There must be exactly 3 blocks between the Start and Finish blocks.


Midi music generator
===

Using the pygame midi module.
To generate Bach-like melodies, learn markov chains from all Bach sonatas. Each markov state is a tuple (pitch, duration). Learn one chain for major scales, and one for minor scales. See http://en.wikipedia.org/wiki/Markov_chain#Music

Driving item-game
===

Drive any kind of vehicle (car, motorcycle, tank, ...). Core gameplay: Mario Kart driving. Long-term gameplay: item game, reuse and salvage parts from other vehicles for improvements to your own. Item game similar to D3 or Plundernauts.



