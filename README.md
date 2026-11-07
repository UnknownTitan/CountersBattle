# Counters

A digital version of the Ghanaian crown-cap flicking game. Each player flicks their cap and tries to land on the other player's cap. Cover half or more of it to score.

The whole game is one file, `index.html`. Open it in any browser to play. No build step and no install.

## How to play

- Press on your cap, pull back and let go. Pull further for a bigger flip.
- Cover half or more of the other cap to score: 1 point, 2 points from 75%, 3 points for a near-full "Gbam" cover. First to 5 wins.
- Cover less than half and the other cap is pinned: its next flick has half power.
- Fall off the table and you miss your next turn.
- 12 seconds per flick. Win two rounds in a row and you are on fire: your next cover earns an extra point.

## Modes

- **Champions ladder:** Kojo (chop bar), Auntie Ama (school veranda), Fitter Yaw (mechanic shop), The Champion (kente cloth).
- **2 players on one phone.**
- **vs computer:** Easy, Medium or Hard.
- **Challenges:** 10 levels with stars.

## Where things live in index.html

- **Physics:** between `/*PHYS*/` and `/*ENDPHYS*/`, with the surfaces (`SURF`) and challenge levels (`LEVELS`).
- **Ladder champions:** `LADDER`.
- **Callout phrases:** `SAY`.
- **Cap designs:** `DESIGNS` and `symbol()`.
- **Places:** `SCENES` and `makeSurface()`.
- **Match rules:** `MATCH`, `CLOCK` and `points()`.

## Roadmap

- Real recorded cap clinks and voice lines.
- Online turn-based 1v1 and WhatsApp challenge links.
- Leaderboards and a daily challenge.
- Android app.
