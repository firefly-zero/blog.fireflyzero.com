---
title: "Making your Firefly Zero game fun"
author: "Gram"
date: "2025-08-30"
tags: ["gamedev"]
draft: true
---

## In short

The best way to make your game fun (or at least memorable) is to **make it unique**. Everyone played Tetris, Snake, or Minesweeper. Give your players something new, give them an unique experience, and they will love your game. And if not for players, do it for yourself. You'll feel more motivated to spend days if not months on a project knowing that you're bringing something new into the world. Make art, not entertainment.

The best wait to make a fun game for Firefly Zero is to make use of things that make the device unique. The main unique features are **multiplayer and touchpad**. No other device takes a good use of touchpad and no other platform makes creating multiplayer games so easy. Your game might not use any of it and still be fun but designing games around multiplayer and/or touchpad is a shortcut to make it special, fun, and memorable.

That's it, that's all you need to know. Below we provie some cool examples of HOW you can use multiplayer and touchpad on Firelfy Zero. The list is not comprehensive but hopefully will inspire you to make your own fun game.

## Multiplayer

### Explore cooperation

[Cooperation](https://en.wikipedia.org/wiki/Cooperation) is a big subject in evolution theory and game theory. The most famous example that you probably is [Prisoner's dilemma](https://en.wikipedia.org/wiki/Prisoner%27s_dilemma). A situation in which it's more benefitial for a group to cooperate but for an individual not to cooperate. Ooooh, work together or betray? Sounds fun. [Robert Axelrod](https://w.wiki/FBZD) in his book [The Evolution of Cooperation](https://en.wikipedia.org/wiki/The_Evolution_of_Cooperation) expanded this experiment into multiple rounds (would you cooperate in this round if you were betrayed on the previous one?) and it's a lot of fun. There are hundreds of different strategies, some are better than others, and [Axelrod-Python](https://github.com/Axelrod-Python/Axelrod) project implemented all of them, and [published results](https://axelrod-tournament.readthedocs.io/en/latest/standard/index.html).

Anyway, what can be more fun to subject your players to hard choices, dilemmas, and social experiments? Maybe mix in some ethical choices, like [Trolley problem](https://en.wikipedia.org/wiki/Trolley_problem).

[Shoot!](https://catalog.fireflyzero.com/lux.shoot) is a very simple demo of the idea. There are enemies attacking the players, and if players kill 30 enemies, they both win. But what if one player kills the other? Then the survivor needs to kill just 5 enemies and there will be only one winner. Ooooh, work together or betray?

### Everything is fun together

You can fun on YouTube and Twitch a ton of streams of people playing junky multiplayer games with their friends and having the best time of their life. It's not that much about playing the game as about doing something together with your friends and sharing the experience.

A simple trick is to get a classic game and ask yourself "can I make it multiplayer?" For many games, like Pong or Snake, the answer is obvious. And for some games, the answer is much more interesting and not obvious at all. Your mind starts to wonder and this is when inspiration strikes. Multiplayer Tetris? Hmmm. You could divide the screen vertically into two parts, let each player control one half, and collapse the line only if it's filled on both sides. Or you could have one play field but let two blocks fall at the same time and each player controls one. Or let one player to only move the block and the other player only to rotate it. So many possibilities! Pick a game you like, write down possible twists you can add, and pick the one that inspires you the most.

[Snek](Music to Make Love to Your Old Lady By) is the very first game we've implemented for Firefly Zero. We've put it together in Go in one evening, glued out first prototypes (Raspberry Pi running [firefly-emulator](https://docs.fireflyzero.com/user/emulator/)), and brought it to our first conference stand. And everyone (including people saying "I don't play video games") had a blast when playing it co-op! People laughing and competing with their friends and families while playing the game we made on the device we made is one of the main memories that I will cherish when I grow old.

### Share through stash

...

## Touchpad

### 360-degrees movement

...

### Rotation

...

### Precision

...

### Intuitive input

...
