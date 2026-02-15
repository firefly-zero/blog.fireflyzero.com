---
title: "Why we're staying on Discord"
author: "Gram"
date: "2026-02-15"
---

## Discord

Shortly after I started working on [Firefly Zero](https://fireflyzero.com/), I registered a bunch of social accounts: Mastodon, Bsky, and Xitter. While I personally only use Mastodon, I want to provide everyone a convenient way to get project updates in their own favorite place. You can contribute to our projects from any OS and IDE, so why should I limit where you get you updates?

Discord followed shortly after, with the same motivation and purpose. I created two channels: `#general` where Discord would post a message for every new person joining (and others would send a "waving hand emoji" to acknowledge the fact) and `#releases` where I would post the same updates as on all other media.

Things had changed when we had our first gamejam. I hired a contractor to handle social media and logistics of the gamejam organization. While I'm a control freak and I still set the gamejam format and some specifics, he had the freedom to write and post any content on any social media without any review. He choose to make Discord the central hub of the gamejam. We created a new `#gamejam` channel and every gamejam announcement on all social media contained an invite to our Discord.

**And it was the right decision**. Not a decision that I'd make myself but a decision that I now believe was right. Instead of just a bunch of people silently making their own game alone in their home, the gamejam turned into a social experience. Even before the gamejam started, people started to share their games and prototypes, ask questions, and socialize. Instead of followers, we now had *a community*. And that's not just useful, it's inspiring. It's one of the little things that keeps us motivate to keep working on Firefly Zero.

## Discord sucks

But as a platform, Discord sucks in a lot of ways. I never used Discord before. If I had a problem that someone already discussed and solved somewhere on Discord, I'd never know about it. Because, unlike Github, Stack Overflow, or forums, nothing from Discord appears in search engines. And if someone somewhere on a forum would say "here is the answer" and post a link to Discord or Slack, I'd just pretend I didn't see it and move on with my life. If you post something exclusively to Discord, it might as well not exist for everyone but a handful of people you're talking to right now.

Another big problem is that Discord isn't your friend. It's a big profit-driven corporation and every profit-driven corporation sooner or later will screw you up to make investors happy. We even have a new word for it: ensittification.

In case you've missed the news, Discord recently reminded everyone about this. They are introducing age verification through government-issued IDs to sell them to USA government just shortly after having a massive data breach. This caused a big exodus from Discord but... Where to go?

## Forums

Forums were a big thing 20 years ago and they are still in use today. For example, Elixir language has a lot of activity on [elixirforum.com](https://elixirforum.com/). Forums are well-structured, searchable, publicly accessible, quite easy to figure out, and easy to self-host and maintain.

The problem with forums is that they don't build a community as well as a instant messaging platform would. Take as an example [the experience](https://sona.pona.la/wiki/Discord#Impact_on_Toki_Pona) of Sonja Lang, the creator of [Toki Pona](https://en.wikipedia.org/wiki/Toki_Pona) conlang:

> But I think a big turning point for the growth of the language was maybe with Discord as a technology. Before that, maybe people were using more forums, or Facebook, or media like that, where the conversation doesn't evolve beyond, 'Hello, where are you from?' 'Oh, yes, how are you? How do you do?' But on Discord, there are live chats happening every day. People are using, reinforcing each other and learning together. That's where I think a lot of the growth came from, from that medium.

So, while solves some problems of Discord, it's not a real replacement. We need something with notifications, solid apps (mobile, desktop, and web), and ability to join and follow multiple communities from one interface. In other words, something that feels like a real messenger, like you're talking to people, not just asking and answering questions.

## Matrix

[Matrix](https://matrix.org/) is the most common place where Discord refugees are migrating. It's non-profit, open-source, cool (end-to-end encrypted), has kinda working moderation, people can join multiple spaces with multiple rooms in each. Sounds perfect.

The problem with Matrix is that it's not accessible for mere mortals. There are multiple clients, each being broken in its own unique way. To log in on a new device or client, it's not enough to know the password, you need to confirm it on another device. Don't have the device where you've created the account? Well, I sure hope you keep the recovery codes! I'm sure there is a very good explanation how it adds an extra layer of security but it's not an inherit problem of encryption: Signal or Proton Mail, for instance, store your private key encrypted on the server and decrypt it on the new device using your password.

And that's just scratching the surface. Firefly Zero isn't just a nerdy FOSS project. It's a game console that anyone can buy and play and for me it's a requirement for our community to be accessible to anyone without taking a cryptography course.

## Zulip

[Zulip](https://zulip.com/) was suggested as one of the first alternatives to Matrix and Discord. It's quite stable, looks nice, has mobile and desktop apps, and some FOSS communities already use it. Another big thing is that it, just like forums, is searchable and accessible from the web without registration.

The problem is that it's more of an alternative to Slack than Discord. Every Zulip "server" has its own hostname, each you need to open in a separate tab, for each you have to create new account, configure it all over again, all that stuff. It's just not designed for communities and people who want to be part of more just one community.

Even if you decide that Firefly Zero is the only community that you want to be part of and you're ready to install an app just for that, you have a new big problem: figuring out how to actually use it. Zulihttps://fluxer.app/p has this creative idea that every message creates its own thread. Which is great for work chats but confusing for most of people and not well implemented. Int other words, Zulip has a very high entry barrier.

## Fluxer and Stoat

[Fluxer](https://fluxer.app/) is the winner in the category "the most familiar UI for Discord refugees". They shamelessly copy the Discord UI as close as possible. You can join multiple communities, each has its own spaces with channels in it, etc. However, FLuxer is a very-very young project. It doesn't have threads yet. When we were trying it out, some people couldn't register. And then the server just crashed, probably not being able to bear the influx of our 5-user community. One day it might be the best Discord alternative but not yet.

Without getting to deep into it [Stoat](https://stoat.chat/) is in a similar situation right now. It looks very promising but at this stage it has too many bugs and stability issues to go all-in with your community.

## IRC

According to Wikipedia, IRC in the past 25 years is steadily dying out and for a good reason: it couln't keep up with the modern demand. It's hard to find a good client, a good server, the only way to make your own space is to self-host a server, there is no file uplaod, and the list of issues goes on. However, considering all the problems we've seen in all other solutions, running an IRC server doesn't seem that crazy.

So, I've deployed an [Ergo](https://ergo.chat/) server, and [ObsidianIRC](https://github.com/ObsidianIRC/ObsidianIRC) web UI for it and it looked kinda nice. You can access the server without registration, you can connect to it using any IRC app, and there is a history of messages. No threads but anyone can make new channels.

And then it started to fall apart. ObsidianIRC is very buggy but it's the only web UI that looks and feels modern (remember, I want something approachable for everyone). I couldn't figure out how to make the server to properly send the chat history to clients. File uploads didn't work. It started to dawn on me that all this complexity, even if solvable, might require me to spend months of setting up and tuning the server and clients. And even if I do that, not many other people will go through the same for their community. So, no, I don't think IRC is the future.

## Telegram and Slack

Telegram and Slack are nice options but they don't solve the main problem of Discord: being at a mercy of an investor-pleasing corporation. No, that's not a route I want to take. I don't want to go through all of this again when a few months later Telegram makes groups over 100 people paid and Slack adds age verification.

## Signal

Signals gains popularity here in Netherlands as an alternative to WhatsApp for small community chats. It's approachable for non-technical people and non-profit. But it doesn't scale well as the community grows: there are no sub-channels and no threads.

## Mastodon

Mastodon is the best modern social technology we have and it already has almost everything you'd want from a Discord alternative. You can go there right now, register on any server (if you haven't already), post anything with `#FireflyZero` hashtag and I and everyone else following the hashtag will see it. I can boost it to get attention of even more people. We can start chatting there in the thread and every time you reply I'll immediately see a notification on my phone. It's fast, distributed, and stable. There is already a Reddit alternative, [Lemmy](https://join-lemmy.org/), that works pretty much like that. They have their own apps that make it look like Reddit but you can still have limited following and participation from a regular Mastodon client. Or take a look at [Pixelfed](https://pixelfed.org/) (alternative to Instagram) or [PeerTube](https://peertube.tv/) (alternative to YouTube) both of which, again, have their own apps but can be used from Mastodon. Cool, huh?

Before I created a Discord server, I hoped that people will just do that but it never happened. I believe the problem is in mentality: you don't really *chat* on Mastodon. You *post* there, *share* what you like, and occasionally *reply*. This mentality leads to the same outcome as with forums: there is activity and following but no community.

Solution? Well, someone needs to go and make a new Discord-like app for Mastodon. I think it's that simple, no need to write your own protocol or server. UI is means to UX. Let people see posts in a hashtag or account as a "community", replies as a "thread", make it look like a messenger, and people will engage with it just like they engage with Discord. Federation is the future and we already have a solid techology ([ActivityPub](https://en.wikipedia.org/wiki/ActivityPub)) for that.

## What's next?

We're staying on Discord because there is nowhere else to go without losing accessbility of our community. I'll keep looking for alternatives and if one day we have a working federated solution, we'll move. Until then, well, let's hope that the new changes don't affect our community.

## Further reading

* [Discord Alternatives: My Personal Deep Dive into Matrix, Zulip, Discourse, and Stoat](https://rant.mvh.dev/discord-alternatives-my-personal-deep-dive-into-matrix-zulip-discourse-and-stoat)
* [Our thread on Discord exploring Discord alternatives](https://discord.com/channels/1291387443089637426/1291387444373229724/1471780993856704576). Yes, it's a link to Discord. If you don't have a Discord account, you're probably not interested in finding a Discord alternative.
