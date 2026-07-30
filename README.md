# Trip Ledger — Settle Up

A single-page web app for splitting group trip expenses. Log who paid for what and who it was shared between, and it works out the minimum number of payments needed to settle every balance.

No backend, no build step, no dependencies to install — it's one HTML file that runs entirely in the browser.

## Features

- Add and remove people on the trip
- Log expenses with description, amount, who paid, who shared it, and date
- Toggle which people share each expense individually (not everyone has to split every cost evenly)
- Automatic balance calculation — who's owed money, who owes into the pot
- Settlement plan that minimizes the number of transfers (e.g. instead of 5 people all paying each other back and forth, it collapses down to the fewest "A pays B" transactions)
- Everything is editable inline, nothing is saved to a server — your data stays in the browser tab

## Usage

Open `trip-ledger.html` in any browser. That's it.

1. Add each person on the trip under **People**.
2. For each expense, add a row: description, amount, who paid, and check off who it should be split between.
3. **Balances** shows each person's net position.
4. **Settle up** shows the shortest list of payments to clear everyone's balance.

## Running locally

```bash
git clone https://github.com/<your-username>/<your-repo>.git
cd <your-repo>
open trip-ledger.html   # macOS
# or just double-click the file in your file explorer
```

## Hosting on GitHub Pages

See the steps in the chat for a walkthrough, or:

1. Push this repo to GitHub.
2. In the repo, go to **Settings → Pages**.
3. Under **Source**, select the `main` branch and `/ (root)` folder, then save.
4. GitHub will publish the site at `https://<your-username>.github.io/<your-repo>/trip-ledger.html`.

## Tech

Vanilla HTML, CSS, and JavaScript. No frameworks, no build tools.

## License

MIT — use it, fork it, change it for your own trips.
