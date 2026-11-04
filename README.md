# Forever Circle — play together

An experimental addon for our friend group: find crafters, share dated character information, request crafts, and save quests to do together.

**Current download: 0.8.0-alpha. Real-game compatibility is still being tested.** Choose the correct client ZIP; everyone testing together should use the same version.

- [Download for WoW Forever](https://github.com/lukevrobbins/forever-circle-downloads/releases/download/v0.8.0-alpha/ForeverCircle-Forever.zip)
- [Download for Classic Era / Hardcore](https://github.com/lukevrobbins/forever-circle-downloads/releases/download/v0.8.0-alpha/ForeverCircle-Classic-Hardcore.zip)
- [Release notes and checksums](https://github.com/lukevrobbins/forever-circle-downloads/releases/tag/v0.8.0-alpha)

Use the named ZIP, not GitHub's automatic Source code archive.

## Install once

1. Close WoW. Extract the ZIP (Windows: right-click → Extract All).
2. Open `ForeverCircle/START-HERE.html` for the Windows/Mac guide, optional local file checker and six feature walkthroughs.
3. In your launcher, select the correct client and open its actual install folder. Copy the whole `ForeverCircle` folder into `Interface/AddOns`.
4. Confirm `Interface/AddOns/ForeverCircle/ForeverCircle.toc` exists, without an extra nested folder. The checker cannot determine whether you chose the actual game installation.
5. Enable Forever Circle in the AddOns list, log in, and use `/fc setup` outside combat. First-run setup also opens automatically.

**Updating:** close the game and back up the old addon and its SavedVariables first. Replace the addon files while retaining saved data. A rollback needs the matching old addon and old data backup. Do not copy saved data between Forever and Classic.

## First five minutes with a friend

- Join the same party. Each player chooses Party in Setup and turns Directory sharing on. Choose Guild later when the guild exists.
- Turn on Location + quests if you want to share whereabouts, quest objectives and waiting notes. Click Sync on both clients.
- Open `/fc home` for quest buddies, orders to review and feature shortcuts. `/fc help` explains each feature; `/fc` opens the directory.
- Open your owned profession windows to collect learned recipes. Search Recipes; no result means not observed, not necessarily unknown.
- Select one of your quests and use Save / edit waiting to leave an explicit plan for friends. Dates show when information was observed; nothing promises someone is online.

## Things you can do

| Goal | Where to start |
|---|---|
| Find a crafter, race/class/level or profession | `/fc` or `/fc find` |
| See last-known locations and shared quests | `/fc whereabouts`, `/fc quests`, or Home → Quest buddies |
| Request a craft | Select a friend's recipe → Request from crafter; both enable order exchange |
| Plan supplies | Select a recipe → Plan materials, then `/fc shopping`; Copy materials shares planned totals manually |
| Coordinate a project, wishlist or activity | `/fc boards`; Directory and Boards sharing both need to be on |
| Learn the controls | `/fc help` |
| Report a problem | `/fc doctor`, plus what you clicked and the first error |

Materials, payment and delivery confirmations stay manual. Message acknowledgment is not acceptance or delivery. Changing audience turns all exchanges off. Previously shared copies can remain with recipients.

## Optional Discord access

In the group's Discord, use `/circle help` for walkthroughs, My characters, quest buddies and sync controls. Automatic sync uses Chrome or Edge, a read-only selected addon SavedVariables file, explicit own-character selection and a revocable connection. Keep the tab active; WoW must save at reload/logout before new observations reach disk. The native Windows picker and real-game save workflow remain acceptance checks.

Manual fallback: `/fc export current`, then `/circle import`. Only own-character observations are exported; other players' caches, inventory, private orders and boards are excluded.

**Addon and Discord orders/activity boards are separate lists.** Create a request in one place and keep its confirmations there. There is no automatic Discord-to-addon import.

## If something goes wrong

Check the same client, addon version, group and both players' sharing settings. Open your own profession before scanning recipes. For stale Discord data, save with `/reload` outside combat and check the sync page. If the addon disrupts play, disable it and reload; retain saved data for troubleshooting.

The offline checker checks the TOC and Lua checksums locally and does not upload or change files. Select only the addon folder, never an account or WTF folder. It validates package files, not game compatibility.

Automated validation: 193 Lua 5.1 checks against source and each extracted client ZIP, 16 install-check cases, six browser-tested walkthroughs, and an eight-client sharing simulation. Actual game APIs, rendering, persistence and delivery still need launch testing. The addon uses no required third-party addons or bundled game assets.
