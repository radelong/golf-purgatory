# Golf Purgatory

A top-down 2D golf game. You died mid-backswing. The afterlife's policy: shoot your declared handicap on the front nine at Purgatory Pines and you move on. Miss it and you play it again.

Your caddie is Dale. He died in 1987. He has opinions.

## Play

Open `index.html` in any modern browser. One file, no install, no build step. Fonts load from Google Fonts and fall back to system fonts offline.

## Controls

| Input | Action |
|-------|--------|
| Click / drag on course | Aim |
| ← → | Fine aim (Shift for finer) |
| ↑ ↓ | Change club |
| Space or Swing button | Three-click swing: start, set power, set accuracy |
| C | Scorecard |
| M | Mulligan (one per round) |
| Enter | Continue on result screens |

## The front nine

| # | Hole | Par | Yards | Gimmick |
|---|------|-----|-------|---------|
| 1 | Orientation | 4 | 360 | None. Enjoy it. |
| 2 | The Lifeguard | 3 | 165 | All carry over a pond; the lifeguard heckles |
| 3 | The Windmill Has Unionized | 4 | 330 | Spinning blades block low shots; periodic strikes |
| 4 | Beach of Regret | 5 | 480 | Bunkers everywhere |
| 5 | Ghost Cart | 4 | 390 | A cart crosses the landing zone and carries your ball off |
| 6 | Lake of Fire | 3 | 190 | Lava carry with a bailout left |
| 7 | The Dogleg of Damocles | 4 | 395 | Hard left dogleg, tall trees in the corner |
| 8 | The Green That Hates You | 4 | 340 | Green slope changes between putts |
| 9 | The Gate | 5 | 520 | Narrow fairway, water left, wind shifts every shot |

## Rules

- Water and lava: one-stroke penalty, drop on the line of entry.
- Out of bounds: stroke and distance.
- Maximum 10 strokes per hole.
- Target score: par 36 plus half your declared handicap (Scratch 36, 9 → 41, 18 → 45, 28 → 50).

Progress saves to the browser's localStorage after each hole, so you can resume a round.
