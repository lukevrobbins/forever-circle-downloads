# Forever Circle downloads

Forever Circle helps a group of friends find crafters, coordinate professions, request crafted items, plan materials, and organize shared projects, wishlists and activities.

## Download

**0.5.0-alpha is an early test build. Automated checks pass; real game compatibility has not yet been verified.** Everyone testing together should install the same version.

- [Download for WoW Forever](https://github.com/lukevrobbins/forever-circle-downloads/releases/download/v0.5.0-alpha/ForeverCircle-Forever.zip) — interface 16001, the build for Forever launch night.
- [Download for Classic Era / Hardcore](https://github.com/lukevrobbins/forever-circle-downloads/releases/download/v0.5.0-alpha/ForeverCircle-Classic-Hardcore.zip) — interface 11509; separate saved data. Hardcore testing is deferred.
- [All releases and notes](https://github.com/lukevrobbins/forever-circle-downloads/releases)

Download the named addon ZIP, not GitHub's automatic **Source code** archive. This repository hosts downloads and installation notes. Each addon ZIP includes readable Lua source; no companion program, website account or Discord bot is required.

## Install

1. Close the game. If updating, back up the existing ForeverCircle addon folder and its SavedVariables first.
2. In the launcher, select the actual game version and open its installation folder. Find `Interface/AddOns`. Classic Hardcore uses the `_classic_era_` installation; use the actual Forever launch installation for Forever.
3. Extract the matching ZIP. The final path should be `Interface/AddOns/ForeverCircle/ForeverCircle.toc`, with no extra ZIP-name folder around it.
4. Launch the game, enable **Forever Circle**, log in, then run `/fc probe` and `/fc` outside combat.
5. Open each owned profession window to collect learned recipes. On Classic, expand the character Skills headers if profession data is unavailable. Recipe knowledge is a dated observation, not a promise the item can be crafted immediately.

Keep the folder named `ForeverCircle`. Retain SavedVariables when updating and do not copy them between game versions.

## Try it with a friend

Join the same normal party. Each player runs:

```text
/fc share party
/fc boards on
/fc orders on
/fc sync
```

Check that you can find each other's character and scanned recipes. Large recipe books can take several minutes. Use `/fc boards` for projects, wishlists and activities, `/fc shopping` for local material plans and `/fc orders` for requests and jobs.

Once you are in the same guild, choose `/fc share guild` and re-enable boards and orders. Changing party membership selects a new group scope; old posts and orders do not move into it automatically.

Order materials, payment and delivery are manual reports. The sender records what was sent and the recipient separately confirms receipt. The addon does not craft, mail, trade or transfer money. Use clearly labeled test orders before relying on it for real requests.

Sharing starts off. To stop all exchanges:

```text
/fc share off
/fc boards off
/fc orders off
```

Previously shared copies remain with recipients. The addon does not upload anything to a website or Discord. `/fc export` copies your own character/recipe observations for an optional future importer; it excludes private orders and board posts.

## Report a problem

Capture the first error, what you clicked, the addon version and `/fc probe` output. Send it to Luke through the group's existing channel. Do not attach account folders, tokens or full SavedVariables to a public issue. If errors interfere with play, disable Forever Circle in AddOns and reload; keep its saved data for diagnosis.

This test build has no automatic updater. Return to the releases page for updates and install the matching ZIP with the client closed.
