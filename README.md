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

## Courses

Pick a course on the title screen. Each keeps its own resume save and best score.

| Course | Difficulty | Holes | Par | Character |
|--------|------------|-------|-----|-----------|
| Purgatory Pines | Original | 9 | 36 | The hand-built front nine (see below) |
| Limbo Links | Easy | 18 | 72 | Wide and forgiving. Nothing happens here. |
| Elysian Fields | Easy | 18 | 72 | Lush parkland, a few ponds, soft greens |
| Brimstone Dunes | Medium | 18 | 72 | Desert links with waste bunkers and lava |
| The Waiting Room Country Club | Medium | 18 | 72 | Ponds, windmills, ghost carts, a heckling lifeguard |
| Styx River Golf Club | Hard | 18 | 72 | Water on nearly every hole, island greens |
| Cerberus National | Hard | 18 | 72 | Doglegs through tight, tall trees |
| The Ninth Circle | Good Luck | 18 | 72 | Ice fairways, the abyss, tiny greens, gale-force gusts. Close to impossible. |

The 18-hole courses are built by a seeded generator with a hand-tuned profile per course (lengths, fairway width, doglegs, hazard types and placement, trees, green size and slope, wind, specials), so every hole is the same each time you play.

### Purgatory Pines (front nine)

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
- Target score: par plus your declared handicap on 18-hole courses, or plus half your handicap on the 9-hole original (Scratch, 9, 18, 28).
- Terrain: fairway, rough, bunkers, green, ice (slides much farther), water, lava and the abyss (all one-stroke penalty hazards).

Progress saves to the browser's localStorage after each hole, so you can resume a round on any course.
