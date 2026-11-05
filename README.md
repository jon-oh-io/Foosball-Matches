# Foosball Tracker: Jon vs Jimmy

A static head-to-head tracker hosted on GitHub Pages. No server, no database: all match data lives in `matches.js`.

## Adding a match

**Option 1: edit the file (always works)**
Open `matches.js`, add a line above `// NEW MATCHES ABOVE THIS LINE`, and commit:

```js
  { date: "2026-11-05", jon: 9, jimmy: 7 },
```

**Option 2: from the web page**
Fill in the "Add a match" form. Without a token, the page shows you the exact line to paste into `matches.js`.
With a token saved (see below), it commits the line for you and the site updates in about a minute.

### Optional: one-click saving
1. GitHub → Settings → Developer settings → Fine-grained tokens → Generate new token.
2. Repository access: **Only this repository**. Permissions: **Contents → Read and write**.
3. On the page, open "Save straight to GitHub", paste the token, click **Save token**.
The token is kept in that browser's local storage only.

## Stats tracked
Wins, win %, current streak, average goals scored and allowed, total goals, goal differential,
average margin of victory, biggest win, and one-goal games.
