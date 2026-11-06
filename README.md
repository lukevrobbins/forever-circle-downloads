# Friends Who Level Together Stay Together — play together

An experimental addon for our friend group: find crafters, share dated character information, request crafts, and save quests to do together.

**Current version: 0.9.1-alpha. Real-game compatibility is still being tested.** Everyone testing together should use the same version.

**WoW Forever: install from CurseForge (easiest).** FWLT is on CurseForge as [Friends Who Level Together Stay Together](https://www.curseforge.com/wow/addons/friends-who-level-together-stay-together). In the CurseForge app, choose World of Warcraft and your Forever installation, search for **Friends Who Level Together Stay Together** and install it. The app then offers each new version as an update. [Already installed from a ZIP?](#switching-from-a-zip-to-curseforge)

**Classic Era / Hardcore, or no CurseForge app:** use the ZIP for your client.

- [Download for WoW Forever](https://github.com/lukevrobbins/forever-circle-downloads/releases/download/v0.9.1-alpha/ForeverCircle-Forever.zip)
- [Download for Classic Era / Hardcore](https://github.com/lukevrobbins/forever-circle-downloads/releases/download/v0.9.1-alpha/ForeverCircle-Classic-Hardcore.zip)
- [Release notes and checksums](https://github.com/lukevrobbins/forever-circle-downloads/releases/tag/v0.9.1-alpha)

[Quick-start infographic (0.8.1 guide; commands still apply)](https://github.com/lukevrobbins/forever-circle-downloads/releases/download/v0.8.1-alpha/FWLT-Quick-Start.png)

Use the named ZIP, not GitHub's automatic Source code archive.

**New in 0.9.1:** sharing keeps to the game's send limit, so it's faster and no longer shows "throttled". It also says what it's doing at the bottom of the Directory, under "What I share" and in chat ("Got Bea's Alchemy: 12 recipes."). In Directory, select a friend and **Browse recipes** to see what they can make. Recipes shows each recipe once with everyone who knows it, and **Request from** sends the request to the friend you pick. "Sync with group" is now **Refresh from group**; sharing runs on its own, so you only need it if something looks out of date. 0.9.0 and 0.9.1 can share data with each other.

**From 0.9.0:** every window is redesigned around one menu on the left (Home, Directory, Together, Orders, Plans and Setup). Only one main page shows at a time, and forms open on top, so windows no longer pile up on each other. Setup is a guided page with an explicit Party / Guild choice, and a "What I share" card shows your sharing at a glance. 0.8.3's **Copy for guild chat** and `/fwlt discord` guide are kept in the new layout. Your saved data, sync and commands are unchanged.

**New name, familiar data:** `/fwlt` is the primary command. `/fc` and `/forevercircle` still work in game. Keep the `ForeverCircle` install folder and saved file; updating uses your existing characters, recipes, orders and settings. Do not install a second folder called FWLT.

## Install from a ZIP

1. Close WoW. Extract the ZIP (Windows: right-click → Extract All).
2. Open `ForeverCircle/START-HERE.html` for the Windows/Mac guide, optional local file checker and seven feature walkthroughs.
3. In your launcher, select the correct client and open its actual install folder. Copy the whole `ForeverCircle` folder into `Interface/AddOns`.
4. Confirm `Interface/AddOns/ForeverCircle/ForeverCircle.toc` exists, without an extra nested folder. The checker cannot determine whether you chose the actual game installation.
5. Enable Friends Who Level Together Stay Together in the AddOns list, log in, and use `/fwlt setup` outside combat. First-run setup also opens automatically.

**Updating a ZIP install:** close the game and back up the old addon and its SavedVariables first. Replace the addon files while retaining saved data. A rollback needs the matching old addon and old data backup. Do not copy saved data between Forever and Classic. CurseForge installs update from the app instead.

## Switching from a ZIP to CurseForge

Your characters, recipes, orders and settings are saved in the game's `WTF` folder, not in the addon folder, so switching keeps them. CurseForge installs the same `ForeverCircle` folder.

1. Close WoW.
2. Back up `WTF/Account/<your account>/SavedVariables/ForeverCircle.lua` (and `ForeverCircle.lua.bak` if present).
3. Move the old `Interface/AddOns/ForeverCircle` folder out of `AddOns`, for example to your desktop. That keeps a copy of the old version and lets the app install cleanly.
4. Install FWLT from the CurseForge app as above.
5. Start WoW, check that Friends Who Level Together Stay Together is enabled in the AddOns list, and run `/fwlt doctor` to confirm the version.

## First five minutes with a friend

- Join the same party. Each player chooses Party in Setup and turns Directory sharing on. Choose Guild later when the guild exists.
- Turn on Location + quests if you want to share whereabouts, quest objectives and waiting notes. Sharing then runs on its own: chat says when a friend's data arrives, and the bottom of the Directory shows progress.
- Open `/fwlt home` for quest buddies, orders to review and feature shortcuts. `/fwlt help` explains each feature; `/fwlt` opens the directory. Use the menu on the left to move between pages.
- Open your owned profession windows to collect learned recipes. In Directory, select a friend and **Browse recipes**, or search Recipes; no result means not observed, not necessarily unknown.
- In Together > Quests, select one of your quests and use **Save / edit waiting** to leave an explicit plan for friends. Dates show when information was observed; nothing promises someone is online.

## Things you can do

| Goal | Where to start |
|---|---|
| Find a crafter, race/class/level or profession | `/fwlt` or `/fwlt find` |
| See last-known locations and shared quests | `/fwlt whereabouts`, `/fwlt quests`, or Home → Quest buddies |
| Request a craft | Directory → select a friend → Browse recipes → pick a recipe → Request from them; both turn on Private orders |
| Plan supplies | Select a recipe → Plan materials, then `/fwlt shopping`; Copy materials shares planned totals manually |
| Coordinate a project, wishlist or activity | `/fwlt boards`; Directory and Boards sharing both need to be on |
| Set up native guild chat after guild creation | `/fwlt discord` or Setup → Native guild chat setup |
| Learn the controls | `/fwlt help` |
| Report a problem | `/fwlt doctor`, plus what you clicked and the first error |

Materials, payment and delivery confirmations stay manual. Message acknowledgment is not acceptance or delivery. Changing audience turns all exchanges off. Previously shared copies can remain with recipients.

## Optional Discord access

Discord uses `/fwlt`. Existing `/circle`, `/craft`, `/orders` and `/lfg` commands still work as aliases. The compact bot name is **Friends Who Level Together**.

In the group's Discord, use `/fwlt help` for walkthroughs, My characters, quest buddies and sync controls. Automatic sync uses Chrome or Edge, a read-only selected addon SavedVariables file, explicit own-character selection and a revocable connection. Keep the tab active; WoW must save at reload/logout before new observations reach disk. The native Windows picker and real-game save workflow remain acceptance checks.

Manual fallback: `/fwlt export current`, then `/fwlt import`. Only own-character observations are exported; other players' caches, inventory, private orders and boards are excluded.

**Addon and Discord orders/activity boards are separate lists.** Create a request in one place and keep its confirmations there. There is no automatic Discord-to-addon import.

## Optional native guild chat

After your guild exists, link Battle.net and Discord accounts and have a guild leader/permitted officer link the intended whole-guild channel. `/fwlt discord` explains the steps and links to the official setup guide. Use `#wow-guild-chat` for human conversation, unlinked `#fwlt` for bot tools, and `#wow-lfg` for activities. Confirm one human message each way after launch. Native chat on Classic/Hardcore remains unverified.

**Copy for guild chat** includes recipe/output identity and quantity for a craft, or title and time for your own current activity. Review the text, then copy and send it yourself. Private terms, price, materials, notes and participants are omitted. Copying creates no order, signup or delivery confirmation. Guild-chat text may appear in linked Discord; choose what you post accordingly.

Native chat does not upload character observations. Keep using browser sync or manual character export for offline lookups. The addon does not connect accounts, detect link status or automatically send chat.

## If something goes wrong

Check the same client, addon version, group and both players' sharing settings. Open your own profession before scanning recipes. If a friend's data looks old, click **Refresh from group**; `/fwlt doctor` shows the sync status and the last send result. For stale Discord data, save with `/reload` outside combat and check the sync page. If the addon disrupts play, disable it and reload; retain saved data for troubleshooting. If windows ever overlap, press Esc to close them and open one again.

The offline checker checks the TOC and Lua checksums locally and does not upload or change files. Select only the addon folder, never an account or WTF folder. It validates package files, not game compatibility.

Automated validation: 227 Lua 5.1 checks against source and each extracted client ZIP, 16 install-check cases, and all 22 runtime files verified by each packaged guide. Previews approximate WoW fonts and controls. Actual game APIs, rendering, persistence and delivery still need testing; 0.9.0 loaded in a Forever client, and 0.9.1 hasn't been tested in game yet. The addon uses no required third-party addons or bundled game assets.
