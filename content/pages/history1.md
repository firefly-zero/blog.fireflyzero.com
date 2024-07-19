---
title: "A brief history of fantasy video game consoles"
author: "Gram"
date: "2024-07-19"
tags: ["software"]
---

This is the first post in the two-part series about the history of Firefly Zero. This post is dedicated to the technologies that inspired Firefly Zero, from early computers to modern programming languages.

## 1977. CHIP-8

In 1977, [Joseph Weisbecker] released [COSMAC VIP]. It was a personal computer designed for writing and playing video games. The whole idea of video games was quite new. [Tetris] was created only in 1985 (8 years after COSMAC VIP). [Pong] was released in 1972, but it was an arcade game, and you would play it on a special big machine designed to run just this one thing. The idea of a computer that is designed for games and can be used to both write and play them was big.

COSMAC VIP was powered by [CHIP-8]. It's a programming language designed to be easy to use (and to learn) and to consume very little memory. It's an interpreted language, which means you can write a command (or modify existing code), press a button, and immediately see the result on the screen. There is no long compilation step or going between computers. CHIP-8 was very fun to use and it still has a [small but passionate community](https://chip-8.github.io/links/) of people writing games for it.

COSMAC VIP also included several games created by [Joyce Weisbecker], the daughter of COSMAC's creator. Most likely, she is the first woman video game developer in history.

We happened to be born decades after CHIP-8 and all these early computers. So, for us, all this old tech, retro games, and early programming languages is more of a fascinating archeological discovery than a childhood memory. And we love them not out of nostalgia but out of appreciation of the engineering beauty, minimalism, and creativity that the constraints of the time sparkled.

[Tetris]: https://en.wikipedia.org/wiki/Tetris
[Pong]: https://en.wikipedia.org/wiki/Pong
[CHIP-8]: https://en.wikipedia.org/wiki/CHIP-8
[COSMAC VIP]: https://en.wikipedia.org/wiki/COSMAC_VIP
[Joseph Weisbecker]: https://en.wikipedia.org/wiki/Joseph_Weisbecker
[Joyce Weisbecker]: https://en.wikipedia.org/wiki/Joyce_Weisbecker

## 2015. PICO-8

[PICO-8] is the first "[fantasy video game console]". "Fantasy" means that there is no actual physical console and never was, only an emulator. It's a virtual machine of sorts that you download on your computer, install, and run. Inside you'll see a text-based terminal, just like in CHIP-8. You type a command, press enter, and immediately see a result. Again, just like on CHIP-8. The programming language is different (Lua) but the ideas are the same: interpreted programming language, interactive text input, designed for both writing and running games. It also comes with an editor for sprites, maps, sounds, and music to give you everything you need for making your own retro game.

PICO-8 has artificial limitations on the screen size, colors used, number of sound channels, and CPU instructions per second. These are here only to ensure the retro feel for every game. There was, however, a project called [PocketCHIP]: a physical pocket-sized computer running PICO-8. Not only games but the whole environment.

The PICO-8 author never mentioned CHIP-8 as inspiration, but they certainly share lots of similarities (including the name). If you are interested in PICO-8 history and roots, check out the first edition of [PICO-8 Zine].

PICO-8 made a big impact on retro game development. There are [more than 5000 PICO-8 games](https://itch.io/games/tag-pico-8) on itch.io, the most famous one being [Celeste](https://en.wikipedia.org/wiki/Celeste_(video_game)#Development), a game made for PICO-8 in 4 days on a game jam. It then was turned into a [full-pledged computer/console game with the same name](https://www.celestegame.com/) that you might've heard of.

[PICO-8]: https://en.wikipedia.org/wiki/PICO-8
[PocketCHIP]: https://en.wikipedia.org/wiki/CHIP_(computer)#Pocket_CHIP_and_Pockulus
[PICO-8 Zine]: https://sectordub.itch.io/pico-8-fanzine-1
[fantasy video game console]: https://en.wikipedia.org/wiki/Fantasy_video_game_console

## 2017. TIC-80

[TIC-80] is one of the many fantasy consoles inspired by PICO-8. The most notable differences are: it's fully open source and it supports lots of programming languages, not just one. There are about 1100 finished games listed on their website. And probably that's all there is to say about it. It's not as influential or notable as PICO-8 but Firefly Zero got a lot of inspiration from it.

[TIC-80]: https://en.wikipedia.org/wiki/TIC-80

## 2021. WASM-4

[WASM-4] is a minimalistic fantasy console that uses [WebAssembly] as a game format. What is WebAssembly? It's a binary format for programs, similar to `.exe` on Windows. The "Web" part in its name means that it is designed to be executed on web pages, just like good old JavaScript, and your browser already supports it for many years. That means you can play any game written for WASM-4 right in the browser.

In terms of features, WASM-4 lags behind PICO-8 and TIC-80: it doesn't have any editors for sprites, music, or sounds. It doesn't even have an interactive prompt like everything else in this post has. And yet, there is still a community of people using it, with [about 120 games published](https://wasm4.org/play) on the website. It is far more than [any other fantasy console](https://paladin-t.github.io/fantasy/index) that we haven't even mentioned. Why so?

That's because games for WebAssembly can be written in lots of languages. The official WASM-4 documentation has code examples for 14 programming languages. And unlike in TIC-80, all of these languages are compiled. Compiled languages are generally faster and can make better use of intentionally constrained resources provided by fantasy consoles.

[WASM-4]: https://wasm4.org/
[WebAssembly]: https://en.wikipedia.org/wiki/WebAssembly

## To be continued

Curious to see how it all ties together? Stay tuned for the second part!
