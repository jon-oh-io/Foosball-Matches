# Office Foosball Tracker

A static head-to-head tracker hosted on GitHub Pages. No server, no database: all match data lives in `matches.js`.

## Adding a player
Open `players.js`, add the name in quotes followed by a comma, and commit:

```js
  "Sarah",
```

## Adding a match

**Option 1: edit the file (always works)**
Open `matches.js`, add a line above `// NEW MATCHES ABOVE THIS LINE`, and commit:

```js
  { date: "2026-11-05", p1: "Jon", g1: 9, p2: "Jimmy", g2: 7 },
```

**Option 2: from the web page**
Fill in the "Add a match" form. Without a token, the page shows you the exact line to paste into `matches.js`.
With a token saved (see below), it commits the line for you and the site updates in about a minute.

### Optional: one-click saving
1. GitHub → Settings → Developer settings → Fine-grained tokens → Generate new token.
2. Repository access: **Only this repository**. Permissions: **Contents → Read and write**.
3. On the page, open "Save straight to GitHub", paste the token, click **Save token**.
The token is kept in that browser's local storage only.

## What's on the page
- **Leaderboard:** every player's games, wins, losses, win %, goals for/against per game, goal differential and streak.
- **Head-to-head:** pick any two players (or click a name on the leaderboard) for their record, stats and match history.
  Link straight to a matchup with `#Jon-vs-Jimmy` at the end of the URL.
- **Recent matches:** the last 25 games across the office.
