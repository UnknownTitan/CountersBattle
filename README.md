# Counters

A digital version of the Ghanaian crown-cap flicking game. Each player flicks their cap and tries to land on the other player's cap. Cover half or more of it to score.

Play it at https://unknowntitan.github.io/CountersBattle/

The game is one file, `index.html`, with a few small files that make it installable. No build step.

## How to play

- Press on your cap, pull back and let go. Pull further for a bigger flip.
- Cover half or more of the other cap to score: 1 point, 2 points from 75%, 3 points for a near-full "Gbam" cover. First to 5 wins.
- Cover less than half and the other cap is pinned: its next flick has half power.
- Fall off the table and you miss your next turn.
- 12 seconds per flick. Win two rounds in a row and you are on fire: your next cover earns an extra point.

## Modes

- **Champions ladder:** Kojo (chop bar), Auntie Ama (school veranda), Fitter Yaw (mechanic shop), The Champion (kente cloth).
- **WhatsApp duel:** play a friend on another phone, one flick at a time. See below.
- **2 players on one phone.**
- **vs computer:** Easy, Medium or Hard.
- **Challenges:** 10 levels with stars.

## WhatsApp duels

There is no server. The whole match travels inside the link.

1. You play your flick. The game builds a link that holds the match: cap positions, bottles, score and whose turn it is, plus your last flick.
2. You send the link on WhatsApp.
3. Your friend opens it, watches your flick replay, plays theirs and sends a new link back.

Each link carries a checksum, so a link that was edited or cut off is rejected. Each phone remembers its duels, so **Your duels** in the menu lets you pick up a match or resend the last link.

## Install

On Android, open the site in Chrome and use **Install the app** in the menu. On iPhone, tap Share, then Add to Home Screen. After the first visit the game works offline.

## Files

- `index.html`: the whole game.
- `manifest.webmanifest`, `icons/`: app name and icons for installing.
- `sw.js`: service worker that caches the game for offline play.

## Where things live in index.html

- **Physics:** between `/*PHYS*/` and `/*ENDPHYS*/`, with the surfaces (`SURF`) and challenge levels (`LEVELS`).
- **Ladder champions:** `LADDER`.
- **Callout phrases:** `SAY`.
- **Cap designs:** `DESIGNS` and `symbol()`.
- **Places:** `SCENES` and `makeSurface()`.
- **Match rules:** `MATCH`, `CLOCK` and `points()`.
- **WhatsApp duels:** the `WhatsApp duels` section (`encode`, `decode`, `receive`, `handOff`).

## Roadmap

- Real recorded cap clinks and voice lines.
- Online ranked play with accounts and ratings.
- Leaderboards and a daily challenge.
- Android app in the Play Store.
