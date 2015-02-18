So many ideas, so little time ...

mogtools
========

Tools for multiplayer online games.
Similar to DirectPlay, but LGPL and cross-platform.
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

Ranker And Match-Maker, based on bots. Purpose: try different MM and ranking algos, unit-testing, and load-testing

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




Mandelbrot, Mandala, and Mondrian
===

Mandelbrot Fractals of Mondrian, like http://kottke.org/11/02/fractal-mondrian

Could also add Mandalas to it.



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


Abbey Manager: REST multiplayer management game using ncurses or tkinter
====

- ncurses: See this list. http://www.use-strict.de/list-of-cool-ncurses-games.html and Curse of War https://www.youtube.com/watch?v=FZH4qbIxpx4
- REST would probably work well for multiplayer games like Drug Wars, Travian, or Football Manager: no real-time interactions, slow gameplay at the scale of hours or days, not seconds.
- theme: the abbey of The Name of the Rose. You are a 14th-century abbot, managing an abbey of 60 monks and 150 servants, with a library, infirmary, church, smithy, brewery, etc. Quotes from the book, p39-41: "it has more books than any other Christian library", "your abbey is the only light that Christianity can oppose to the thirty-six libraries of Baghdad", "many of the monks living in your midst come from other abbeys scattered all over the world. Some stay here a short time, to copy manuscripts to be found nowhere else, not without having brought you some manuscript or great rarity in exchange. Others stay here for a very long time because only here can they find the works that enlighten their research.", "Only the librarian knows where to find a book in the labyrinth of the library, which truths and falsehoods it contains, and who should or should not read it."
- Could have time-based mechanics. 
- Farmville meets Agricola: resource production more customizable/complex than Farmville, synergies within your resource productions and consumptions more abundant than in Agricola.
- Abbey = inn + church + library. Thus 3 currencies. 1) Each transaction happening inside the inn generates gold. Selling veggies or animals brings gold too. Gold is spent on new buildings, seeds, animals, and relics. Use gold to buy favors from the King (eg mercenaries/militia to protect from thugs and beasts). 2) Pious monks praying in the church generate piety. Abbey piety cap is the sum of the praying monks' piety. Piety decreases and increases slowly (whether below or above cap). The Pope can sanctify very pious monks or send Inquisitors against those he considers heretics. 3) Knowledge is acquired by copying books, storing them in library, and adequately hosting scholars from the entire world. The more erudite your abbey, the more your Order will direct scholars to visit it.
- Overall, the King prefers an abbey that is rich (and skeptic), the Pope pious (and ignorant), and the Order erudite (and poor). The King hates the Order which hates the Pope who hates the King.
- Friars vs monks vs nuns vs ... http://en.wikipedia.org/wiki/Category:Ecclesiastical_titles
- Each Order has particular rules and tradeoffs: Benedict (respect of the hierarchy), August (mendicants), Albert (= the Carmelite mendicants), Franciscans (minority and penance), Cistercian (manual labour and self-sufficiency), Trappist, Carthusian, Pachomius, Cluniac, ...




Shadow of the Colossus/Monster Hunter in 2D
===

- Get a bounty for a monster, kill that monster, receive bounty reward, improve gear, get higher bounty, repeat.
- Each monster has a particular behavior, eg a crab moves sideways and can only be attacked from behind.
- Top-down graphics like old Zelda. Maybe the code from crowd-control could work for that. 



Map generator
===

Like Diablo or roguelike games. Maps are made of at most 10 blocks of 50x50 cells. Each block can have up to 4 gates, eg a North gate is a hole from 24,0 to 25,0, and the rest of row 0 are walls. Each block must have at least one gate. Blocks can be hand-made or generated. There must be exactly 3 blocks between the Start and Finish blocks.

Check: Adventures in Level Design from Joris Dormans, PCG workshop from FDG, and Automatic Generation of Dungeons
for Computer Games from David Adams.



Midi music generator
===

Using the pygame midi module.
To generate Bach-like melodies, learn markov chains from all Bach sonatas. Each markov state is a tuple (pitch, duration). Learn one chain for major scales, and one for minor scales. See http://en.wikipedia.org/wiki/Markov_chain#Music


Driving item-game
===

Drive any kind of vehicle (car, motorcycle, tank, ...). Core gameplay: Mario Kart driving. Long-term gameplay: item game, reuse and salvage parts from other vehicles for improvements to your own. Item game similar to D3 or Plundernauts.


Builder/assembler item-game
===
Building a complex system (computer, car, boat) from hardware parts requires knowledge of constraints, synergies, and co-requirements. Theme: you own a shop where customers want to buy a system with particular features (eg latest graphics card or low power consumption). Core loop: optimize a build by selecting the best/cheapest parts that synergize well. Like http://pcpartpicker.com. Could add an auction house to it. Long loop: make profits from selling systems, unlock new parts from manufacturers, gain a customer rep (eg super cheap but often breaks, great customer service but overpriced), and gain manufacturer rep (sell Nvidia and AMD won't talk to you).


Stories for data scientists
===

Instead of sentences, give data. Both can tell stories equally well. Both can have bias and be interpreted differently by different readers.


Psychology for game designers
===

a book


Game theory for game designers
===

a book


Machine Learning tutorials
===

Explain the basic idea of each algorithm. Give R code. Provide examples where each works best, and where each sucks. Check Max Welling's slides. http://www.ics.uci.edu/~welling/teaching/ICS273Afall11/ICS273Afall11.html
