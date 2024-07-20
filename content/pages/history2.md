---
title: "Bringing WebAssembly to microcontrollers"
author: "Gram"
date: "2024-07-19"
tags: ["software"]
draft: true
---

This is the second and the last part in the series about the history of Firefly Zero. First part: [A brief history of fantasy video game consoles](./history1.md).

## 2017. WebAssembly

We already touched a bit on WebAssembly in the first part. It was released in 2017. I started to work with WebAssembly in 2019. At the time, the only thing I knew about it is that it's a way to write frontend code in the Go programming language instead of JavaScript. And since JavaScript is somewhere at the bottom of my top of programming lanugages, that was enough of a reason for me to start using WebAssembly with Go.

One of the first thing I did is I created [gweb](https://github.com/life4/gweb). It's a tool that makes it possible to do in Go everything you could do in JavaScript. I also made [quite a few demos](https://gweb.orsinium.dev/) for it. My favorite one is [Breakout](https://gweb.orsinium.dev/breakout/), an improved port of the classic video game with the same name. You can click the link and play it right in your browser. But beware, it's quite addictive.

The next benefit of WebAssembly I discovered, besides writing JavaScript-free frontend, is that you could run in the browser existing games and tools with almost no modifications. I started to make online playgrounds for my Python projects:

* [svg.orsinium.dev](https://svg.orsinium.dev/): a playground for [svg.py](https://github.com/orsinium-labs/svg.py), a Python library for generating SVG images.
* [wps.orsinium.dev](https://wps.orsinium.dev/): a playground for [wemake-python-styleguide](https://github.com/wemake-services/wemake-python-styleguide), a tool for finding bugs in Python code.

And some people were pushing it even further. Here are a few of my favorite browser ports:

* [DOOM](https://silentspacemarine.com/)
* [Windows 95](https://archive.org/details/win95_in_dosbox)
* [Gameboy](http://binji.github.io/binjgb/) (you'll need a ROM to play, [download one here](https://www.emulatorgames.net/roms/gameboy/))

## 2023-11. Aard

In November 2023, I started to write a programming language.

## 2024-02. TinyGo

...

## 2024-02. Gamgee

...

## 2024-03. Firefly Zero

On 10 March 2024, I met with Alex, told him about the same history as you just read, and said that I want to make a handheld game console with WebAssembly and multiplayer. The very next day we started to write the first documentation for what will later become Firefly Zero. I drafted some design ideas for graphics and Alex wrote down what hardware components we will need. This was the beginning.

At the moment of writing this post (July 2024), we already made a lot of progress, especially considering that we both have daily jobs and work on Firefly Zero on evenings and weekends. We have SDKs for Go and Rust, drafts for SDKs for Python, C, C++, Zig, and Elixir, a very powerful CLI, online game catalog, testing framework, cross-platform emulator, graphics, and even multiplayer. If we are pressed to release the project as-is in this very minute, we already wouldn't be ashamed of the result. And yet, we still have a lot of things we want to implement before that. This is our first big project, and we want it to be very good and memorable.

Show must go on!
