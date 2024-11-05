# UBlock-Origin allowlist
UBlock-Origin Javascript filter list, to make the switch easier for everyone

[🇩🇪 deutscher Text](https://github.com/boredsquirrel/ublock-allowlist/blob/main/README-deutsch.md)

This repo contains "UBlock Origin dynamic filtering rules". Basically, it is a better replacement for [NoScript](https://noscript.net)

## Goal
UBlock-Origin works well as an adblocker, using "badness enumeration" with huge lists of bad domains. But this concept is flawed, so for real security, users need to

1. Block every executable code by default
2. Unblock every site they trust

This project is there to make this less painful, by offering a big list of trusted domains, a "small internet" so to say.

## Bias of this list
I am a german guy, interested in tech and science stuff. That is pretty obvious in the filterlist, which is basically my browsing history (*I hope you appreciate that*).

You are free to add whatever site you like to reduce this bias, but please follow a few rules.

## Rules

### 1. Images are allowed

### 2. All Javascript is blocked by default
This includes 1st and 3rd party javascript.

### 3. No origins are blocked
URLs are only allowed if you trust them. Double-blocking doesn't do anything.

### 4. How to allow
UBlock Origin shows 2 columns:

![screenshot](https://github.com/boredsquirrel/ublock-allowlist/blob/main/images/ubo-popups.jpg?raw=true)

The left column applies to any site, e.g. "load `google.com` Javascript on any website". The right column applies to the currently opened site, e.g. "load `google.com` javascript only on `youtube.com`.

When unblocking, limit known surveillance origins (like Google, Facebook, Amazon etc) to their own homepages.

To make the list shorter, you can unblock random website javascript in the left column, as that is "trusted" and not loaded on other sites.

### 5. What to unblock
Security is a balance between "everthing loads whatever it wants" and "I see a blank page".

This means that many CDNs and other centralized actors on the web need to be unblocked, as a ton of websites rely on them.

But experiment, dont just unblock everything. A few missing images can be fine, and some may not even load anything useful, but just analytics etc.

## How to setup
1. Install UBlock Origin, this means you need Firefox or a Firefox-based Browser (Mull, Torbrowser, MullvadBrowser, Midori, Floorp, Zen...)
2. In the UBO Settings, enable "advanced mode"

![screenshot](https://github.com/boredsquirrel/ublock-allowlist/blob/main/images/ubo-advanced-enable.jpg?raw=true)

3. Now you can import this list under "My Rules"
4. Open some websites, using the Addon popup (see first screenshot) you can unblock javascript
5. These unblocks are temporary !!! (For whatever reason). Go to the UBO Settings page, "My Rules" and "Commit" your changes to the list

![screenshot](https://github.com/boredsquirrel/ublock-allowlist/blob/main/images/ubo-settings.jpg?raw=true)

## How to contribute
Once you have this setup, you can unblock more trusted origins and commit the changes.

UBO will make a neat list out of this.

1. Fork this repo
2. Make sure you use the up-to-date list as base, otherwise changes may be lost
3. In your fork, just use the Github Web Editor and edit the blocklist
4. Replace the entire content with your new list
5. Commit, creating a new branch. Use a random name for that branch
6. Go back to this repo, not your fork
7. Use the popup in Github, to create a PR, from your fork and branch, to this repo and the `main` branch
8. Write a few words, and we can merge it quickly!
