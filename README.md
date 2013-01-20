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
