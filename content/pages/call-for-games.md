---
title: "Call for games"
author: "Gram"
date: "2024-12-21"
tags: ["software"]
---

We're making a cool game console and we need you to make cool games for it.

[Firefly Zero](https://fireflyzero.com/) is a handheld game console, similar to [Game Boy Advance](https://en.wikipedia.org/wiki/Game_Boy_Advance) (GBA). However, unlike GBA, it is modern (and easy to program), has same-room multiplayer (over Bluetooth), and uses a touchpad instead of D-pad for more precise controls.

## Developer experience

Firefly Zero is a game console with the best developer experience. It is the first WebAssembly-powered handheld game console in the world. All you need to know about WebAssembly is that it is supported by almost all modern programming languages. And you can use any of them for writing Firefly Zero games!

Already supported:

* [Go](https://github.com/firefly-zero/firefly-go)
* [Rust](https://github.com/firefly-zero/firefly-rust)
* [C and C++](https://github.com/firefly-zero/firefly-c)
* [Elixir](https://github.com/firefly-zero/firefly-elixir) (experimental)

In future, we'll support Python, TypeScript, Lua, Zig, Kotlin, and much more.

The official SDKs are designed to be idiomatic, friendly, and zero-allocation.

Firefly Zero has [firefly-cli](https://github.com/firefly-zero/firefly-cli) a swiss army knife CLI tool to do everything you'll ever need for writing a game: build, publish, download, install, profile, inspect, etc.

Creating your first app is as simple as:

```bash
firefly_cli new --lang=rust hello-world
firefly_cli build
firefly_emulator
```

The [desktop emulator](https://docs.fireflyzero.com/user/emulator/) runs exactly the same runtime as the real device. If it works on emulator, it will work on the device.

You can read more about getting started in the [documentation](https://docs.fireflyzero.com/dev/getting-started/).

## The new frontier

Now is the best time to make a game for Firefly Zero:

1. We have [an official game catalog](https://catalog.fireflyzero.com/) which is currently has just a few games. Every early adopter will see and play your game.
1. With the permission of authors, we'll include (keeping the author's name and all attributions) the best games on the device by default. Everyone who ever buys the device will play your game.
1. We will also pay you for including your game on the device. We want to support your work as you support ours.
1. We'll have a stand at [FOSDEM 2025](https://fosdem.org/2025/) where we will show the first prototypes running the community games. FOSDEM is on 2025-02-01, so, naturally, we will only showcase the games that are working (not necessarily finished) by that date.
1. We'll make sure that all early adopters, including early gamedevs, will be the first to receive the finished product.

## Getting paid

There are 3 ways how you can make a buck from your game:

1. **Hobbyist**. Work in your own pace and do whatever you want. If the game is fun to play, we buy it from you and preinstall on all devices.
1. **Enterpreneur**. Make a commercial game and sell it as you want, for any price on any platform. If you lend us a free copy of the game, we'll include it on prorotypes that we show on conferences, so that people can try it out. And in general, we will do our best to promote your work as any other community game.
1. **Freelancer**. Pitch us your game and tell us how long it will take to get it working. If it sound good, we'll pay you 20 euro/hour for your work. If you want more (or less), let's talk. We'll give preference to the games that can be done before FOSDEM.

In all cases, we will provide you first-class support: if you're stuck with anything, just send us in Telegram any questions you might have, and we will help you.

## Inspiration

There are already a few FOSS games for Firefly Zero:

* [Snek](https://github.com/firefly-zero/snek) (Go)
* [Flappy Gopher](https://github.com/deadprogram/flappy-gopher) (Go)

More games will be added over time, so keep an eye on [catalog.fireflyzero.com](https://catalog.fireflyzero.com/). Pro tip: you can browse the catalog from terminal: `firefly_cli catalog list`.

A good starting point is to port an existing game. And then maybe add a twist on it, like multiplayer or more precise controls with the touchpad.

[WASM4](https://wasm4.org/play) is one of the closest platforms to Firefly Zer oin terms of supported API. Its catalog has lots of games, many of which are open-source. Some of my favorites:

* Go:
  * [2048](https://github.com/peterhellberg/w4-2048)
  * [Tic Tac Toe](https://github.com/christopher-kleine/tic-tac-toe-wasm4)
* Rust:
  * [Kitty Game](https://github.com/canyonturtle/kittygame)
  * [Dodgeball](https://github.com/SLiV9/dodgeball-wasm-4)
* C:
  * [Watris](https://github.com/aduros/wasm4/tree/main/examples/watris)
  * [Waternet](https://github.com/joyrider3774/waternet_wasm4)

If you like programming in C, you can look into porting an existing emulator for a retro game console. For example, an emulator for GBA (which, BTW, has the same screen size, 240x160 pixels). You port one emulator, and you can now run hundreds of existing classic games! How cool is that?

Lastly, somebody will eventually port DOOM to Firefly Zero. You can be the first one.

## Next steps

Go to [Getting started](https://docs.fireflyzero.com/dev/getting-started/) documentation and follow the steps to get your first app running. If you have any questions or want to get paid, drop us a message:

* Discord: [discord.gg/fx4Wmn6DwD](https://discord.gg/fx4Wmn6DwD)
* Telegram: [@orsinium](https://t.me/orsinium)
* Email: [firefly@orsinium.dev](mailto:firefly@orsinium.dev)
