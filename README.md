# Friends Who Level Together Stay Together — play together

An experimental addon for our friend group: find crafters, share dated character information, request crafts, and save quests to do together.

**Current version: 0.11.0-alpha. Real-game compatibility is still being tested.** Everyone testing together should use the same version.

**WoW Forever: install from CurseForge (easiest).** FWLT is on CurseForge as [Friends Who Level Together Stay Together](https://www.curseforge.com/wow/addons/friends-who-level-together-stay-together). In the CurseForge app, choose World of Warcraft and your Forever installation, search for **Friends Who Level Together Stay Together** and install it. The app then offers each new version as an update. [Already installed from a ZIP?](#switching-from-a-zip-to-curseforge)

**Classic Era / Hardcore, or no CurseForge app:** use the ZIP for your client.

- [Download for WoW Forever](https://github.com/lukevrobbins/forever-circle-downloads/releases/download/v0.11.0-alpha/ForeverCircle-Forever.zip)
- [Download for Classic Era / Hardcore](https://github.com/lukevrobbins/forever-circle-downloads/releases/download/v0.11.0-alpha/ForeverCircle-Classic-Hardcore.zip)
- [Release notes and checksums](https://github.com/lukevrobbins/forever-circle-downloads/releases/tag/v0.11.0-alpha)

[Quick-start infographic (0.8.1 guide; commands still apply)](https://github.com/lukevrobbins/forever-circle-downloads/releases/download/v0.8.1-alpha/FWLT-Quick-Start.png)

Use the named ZIP, not GitHub's automatic Source code archive.

**New in 0.11.0: Your Story.** A private notebook of your character's adventure fills itself in as you play. Open **Your Story** from the left menu, **Discover your story** on Home, or `/fwlt story`. **Discover** shows this login's chapter, a recent standout and your personal records. **Moments** lists first finds and crafts, quest turn-ins, new levels, deaths and returns, and "Finally!" when a drop you were tracking in Field Stats turns up after a long dry streak. **Passport** stamps each new map, **Company** remembers who you grouped with, and **Keepsakes** keeps up to 30 favorite moments. It records from now on, not your past, and nothing in it is shared. Turn it off on the page or in Setup → Preferences.

**From 0.10.0: auction prices, Field Stats and preferences.** On Forever, FWLT remembers the auction prices of listings you open at an auctioneer, and **Look up materials** in Shopping or Plan materials checks prices one item at a time. Shopping then estimates what your missing materials cost, and Plan materials compares them with the crafted item's lowest listing. Prices stay on your computer for 30 minutes. `/fwlt stats` opens **Field Stats**, a notebook of what you loot, craft and earn from quests; link a quest item to its objective to see how often it drops for you, and share summaries with your group only if you turn that on. **Setup → Preferences** (`/fwlt settings`) turns the party sound, interface sounds, hints, chat notices, the minimap button and the mail and trade helper on or off. Plans show your pledge or signup and progress on each row, a chat line tells you when it's your move, Orders lists your moves first, results appear as a notice on the page, and lists show item, profession and class icons.

**From 0.9.9: a party join sound, easier browsing and item rows.** A sound plays when a friend joins your party or you join theirs (Nick's John Cena clip): `/fwlt cena off` turns it off, `/fwlt cena on` turns it back on and `/fwlt cena test` plays it. **Fully close and restart WoW after updating** so the new sound file loads. Plan forms list items as rows with their own quantities: Shift-click or paste an item, set the quantity, then **Add item**. Recording what you received starts with a searchable list of contributors, and quest waiting notes you haven't saved stay on your computer as drafts. In the search box of any list, Up and Down move through the results and Enter opens one; hovering a row shows its full text. Recipes shows **Reset filters** when a filter is on, and Plans and Shopping find plans by material name or item ID. Setup is split into sections, the crafting request shows the whole form at normal size, Directory's profession and crafter choices are searchable lists, and the mail and trade helper pages through all your orders.

**From 0.9.8: what needs you comes first.** Home opens on a **What needs you** list: orders where it's your move, friends waiting for you on a shared quest and new replies on your posts, each with a button that opens it. New replies stay counted until you click their post (just opening Plans no longer clears them), and each post shows "2 new". Crafting requests keep what you typed when you close them, switch pages or `/reload`, with **Keep draft** and **Discard**; Setup keeps unsaved nickname and profession-goal edits until you save or discard them. On small screens or with a large UI scale, Home, Directory, Together, Plans and Orders show the list first, then the details, with **Back to results**. Quest buddies shows your current group unless you choose **Include earlier groups**. Replies you got before updating may show as new once.

**From 0.9.7: see what needs you.** Small amber counts on the left menu show orders waiting on you (Orders), friends waiting for you on a quest (Home) and new pledges or signups on your posts (Plans); hover one to see what it means. The minimap button shows the total. Order rows say where each order stands ("Materials 6/16", "Delivered 2/4"). Together → Quests gives each person a heading with progress bars for their objectives, and item names now fill in instead of showing "Item 2589".

**From 0.9.6: recipe gift hints** (thanks, Nick). Hover a recipe item in your bags, at a vendor or in an FWLT window, and a small FWLT bubble under the tooltip says whether someone could use it: **Gift this!** with the friends who may need it, **Keep this!** when only your alts may, or **No known need · 2 not scanned** when some characters haven't shared a full scan. "Looks like nobody needs this" appears only when everyone with that profession was checked. It's worked out on your computer from shared scans and sends nothing; `/fwlt gifts off` hides it.

**Also from 0.9.6:**

- **`/fwlt` opens Home**, like the minimap button. `/fwlt directory` opens the Directory and `/fwlt find` still searches recipes.
- **Plan drafts are kept.** A new project, wishlist or activity keeps what you typed if you close it, switch pages or reload. **Keep draft** and **Discard** replace Cancel.
- **Earlier party plans stay visible** as saved history when someone joins or leaves the party, and you can copy your own open post to the new party.
- **Readable on small screens.** If a window doesn't fit, it keeps normal text size and scrolls, instead of shrinking.

**From 0.9.3 to 0.9.5** (CurseForge had 0.9.3 and 0.9.4 in between):

- **Smoother windows (0.9.3).** Lists scroll smoothly instead of jumping a page at a time. Escape closes the top FWLT window, Enter saves a form, and shift-clicking an item fills it in. The window remembers where you put it, and a minimap button opens FWLT.
- **Plain wording (0.9.3).** No internal numbers on screen, one name for each sharing switch, plain order status and quieter chat. `/fwlt help` prints a short list; `/fwlt notices off` quiets sharing notices.
- **Visual details (0.9.4).** Details show items with their icons and tooltips, and progress bars for order materials, plan goals, your shopping list and profession skill. Crafting requests list materials as rows you can edit. Orders details use the whole column.
- **Settings in Setup (0.9.4).** The four sharing switches and your nickname and profession goals live in Setup; a badge in each window's header shows who you share with and whether sharing is working.
- **Reviewed fixes (0.9.5).** After a reload the status says **Saved data only** until friends are heard from again. Quest buddies seen recently come first. Paused shopping plans no longer block new ones and can be deleted. Party orders keep working when someone joins or leaves the party; for that, both players need 0.9.5.

**From 0.9.2:** each crafting order shows a step bar (Requested → Accepted → Materials → Crafting → Delivered → Paid → Done) and one-click buttons for your next move, such as **Confirm 4 received** or **I paid 2g**. At a mailbox or trade window, an FWLT panel can fill in what an order still needs: click **Attach**, press Send yourself, then **Record**. Whether the game lets addons move items into mail is still being tested; if it doesn't, the panel says so and you drag items in as before.

**From 0.9.1:** sharing keeps to the game's send limit, so it's faster and no longer shows "throttled". It also says what it's doing at the bottom of the Directory, in the header badge and in chat ("Got Bea's Alchemy: 12 recipes."). In Directory, select a friend and **Browse recipes** to see what they can make. Recipes shows each recipe once with everyone who knows it, and **Request from** sends the request to the friend you pick. "Sync with group" is now **Refresh from group**; sharing runs on its own, so you only need it if something looks out of date. 0.9.0 and 0.9.1 can share data with each other.

**From 0.9.0:** every window is redesigned around one menu on the left (Home, Directory, Together, Orders, Plans and Setup). Only one main page shows at a time, and forms open on top, so windows no longer pile up on each other. Setup is a guided page with an explicit Party / Guild choice, and a "What I share" card shows your sharing at a glance (since 0.9.4, a badge in the header). 0.8.3's **Copy for guild chat** and `/fwlt discord` guide are kept in the new layout. Your saved data, sync and commands are unchanged.

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
- Turn on Together sharing in Setup if you want to share whereabouts, quest objectives and waiting notes. Sharing then runs on its own: chat says when a friend's data arrives, and the bottom of the Directory shows progress.
- Open `/fwlt home` for quest buddies, orders to review and feature shortcuts. `/fwlt` and `/fwlt home` open Home, `/fwlt directory` opens the directory, and `/fwlt help` explains each feature. Use the menu on the left to move between pages.
- Open your owned profession windows to collect learned recipes. In Directory, select a friend and **Browse recipes**, or search Recipes; no result means not observed, not necessarily unknown.
- In Together > Quests, select one of your quests and use **Save / edit waiting** to leave an explicit plan for friends. Dates show when information was observed; nothing promises someone is online.

## Things you can do

| Goal | Where to start |
|---|---|
| Find a crafter, race/class/level or profession | `/fwlt directory` or `/fwlt find` |
| See last-known locations and shared quests | `/fwlt whereabouts`, `/fwlt quests`, or Home → Quest buddies |
| Request a craft | Directory → select a friend → Browse recipes → pick a recipe → Request from them; both turn on Orders sharing in Setup |
| Send materials or deliver | At a mailbox or trade window, use the FWLT panel: Attach, press Send yourself, then Record. Or follow the order's "Your move" buttons |
| Plan supplies | Select a recipe → Plan materials, then `/fwlt shopping`; Copy materials shares planned totals manually |
| Coordinate a project, wishlist or activity | `/fwlt plans`; Directory and Plans sharing both need to be on |
| Set up native guild chat after guild creation | `/fwlt discord` or Setup → Guild chat in Discord |
| Check whether a friend needs a recipe | Hover the recipe item; `/fwlt gifts off` hides the hint |
| See what needs you | Home's What needs you list, plus the amber counts on the left menu and minimap button |
| Turn the party join sound off or on | `/fwlt cena off` or `/fwlt cena on`; `/fwlt cena test` plays it |
| Choose sounds, hints, chat notices and helpers | `/fwlt settings` (Setup → Preferences) |
| Estimate material costs (Forever) | At an auctioneer: Shopping or Plan materials → Look up materials |
| Keep a loot notebook or study a quest drop | `/fwlt stats` |
| See your character's story, firsts and keepsakes | `/fwlt story` |
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

Automated validation: 508 Lua 5.1 checks against source and each extracted client ZIP, 20 install-check cases, and all 35 runtime files verified by each packaged guide. Previews approximate WoW fonts and controls. Actual game APIs, rendering, persistence and delivery still need testing; 0.9.0 loaded in a Forever client; 0.9.1 to 0.11.0 haven't been tested in game yet. The addon uses no required third-party addons or bundled game assets; its one sound file is the party join clip.
