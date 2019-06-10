# Meritous

Branch|[![Travis CI logo](pics/TravisCI.png)](https://travis-ci.org)
---|---
`master`|[![Build Status](https://travis-ci.org/richelbilderbeek/meritous.svg?branch=master)](https://travis-ci.org/richelbilderbeek/meritous)

Meritous is one of my favorite open-source games. 
It is programmed in C using the SDL. 
Because the game is open-source, 
I could obtain much information from the code.

## Strategy guide

There are three skills:

 * Shield: the size of you shield
 * Circuit charge rate: the speed of which your psi circuit charges
 * Circuit recharge rate: the speed of which your psi circuit recharges after a psi shot

The three skills can be upgraded for an increasing price, dependent on current skill level and mode. For this formula and prices, see below. Increasing shield level is more expensive then a circuit (re)charge upgrade. Circuit charge and circuit recharge upgrade cost as much. The maximum skill level is 24. The Agate knife takes all your skill levels to 24.

 * The maze is generated at random, so there is no need to post a map
 * You do not need waste time to pick up crystals: a crystal generator gathers all crystals in the maze in one room
 * When you have enough crystals to upgrade one of your stats (Reflect shield, circuit charge, cicuit refill), these words are highlighted
 * A good tactic is to fight monsters until one of your skills is highlighted. Then find a teleporter to the main starting room. Use the crystal generator there and buy your upgrade
 * Collect all the non-essential artifacts first. When you encounter a compass, the dark-grey arrow points to a non-essenstial artifact. When there is no grey arrow, you have found all non-essential artifacts
 * When you finish a boos room, save your progress before opening the chests. In one chest, there will be an artifact. In the others, there might be a shield/charge/refill improvement. Wait with collecting these until you cannot make these upgrades by gathering crystals anymore. In other words: a level one shield upgrade costs only 50 crystals, a level 10 upgrade about one million, so let those upgrades ripen
 * Each time you kill a boss, all monsters get tougher. Kill the bosses after exploring all rooms
 * Clear all rooms to obtain the Agate knife. Kill the three bosses last, so that at the third boss, you will obtain it. You do not need to kill all creatures in the dungeon
 * You do not need to kill all creatures in the dungeon
 * There is no cheat-mode (it is commented out of the source code)

```
shield price = ((100 - 50*m) * s) + ((5*2^s) * (5 - 2*m))
s = current shield level
m = mode = 0 for wuss mode, 1 for normal mode
```
 
Shield level | Wuss mode | Normal mode mode
---|---|---
0 | 15 | 25
1 | 80 | 150
2 | 160 | 300
3 | 270 | 500
4 | 440 | 800
5 | 730 | 1300
6 | 1260 | 2200
7 | 2270 | 3900
8 | 4240 | 7200
9 | 8130 | 13700
10 | 15860 | 26600
11 | 31270 | 52300
12 | 62040 | 103600
13 | 123530 | 206100
14 | 246460 | 411000
15 | 492270 | 820700
16 | 983840 | 1640000
17 | 1966930 | 3278500
18 | 3933060 | 6555400
19 | 7865270 | 13109100
20 | 15729640 | 26216400
21 | 31458330 | 52430900
22 | 62915660 | 104859800
23 | 125830270 | 209717500
24 | 419432800 | 251659440

```
circuit (re)charge price = ((100 - 50*m) * c) + ((5*(2^c)) * (5 - (2*m)))
c = current circuit (re)charge level
m = mode = 0 for wuss mode, 1 for normal mode
```

Circuit (re)charge level | Wuss mode | Normal mode mode
---|---|---
0 | 10 | 20
1 | 60 | 120
2 | 120 | 240
3 | 200 | 400
4 | 320 | 640
5 | 520 | 1040
6 | 880 | 1760
7 | 1560 | 3120
8 | 2880 | 5760
9 | 5480 | 10960
10 | 10640 | 21280
11 | 20920 | 41840
12 | 41440 | 82880
13 | 82440 | 164880
14 | 164400 | 328800
15 | 328280 | 656560
16 | 656000 | 1312000
17 | 1311400 | 2622800
18 | 2622160 | 5244320
19 | 5243640 | 10487280
20 | 10486560 | 20973120
21 | 20972360 | 41944720
22 | 41943920 | 83887840
23 | 83887000 | 167774000
24 | 335546240 | 167773120

## External links

 * [Meritous homepage](http://asceai.nfshost.com/meritous/)