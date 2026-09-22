# THE TAPE — upload rules

Never ship a stub, wrapper, iframe, or `filename (1).html` as the live page.

## File names
- Home / OPEN: `index.html` only.
- Watchlist: `watchlist.html`
- Ledger: `ledger.html`
- Results: `results.html`
- Ticker dive: `YYYY-MM-DD-TICKER.html`  Example: `2026-09-23-CAT.html`
- If a download creates `file (1).html`, copy onto the real name, then delete the `(1)`.

## Every ticker dive must include, in this order
1. One header bar: OPEN · WATCHLIST · LEDGER. Not stacked sticky bars. No iframe.
2. THE TAPE / date / ticker / full name / LOCKED 9:10 or OPEN. No version stamp in the header.
3. Four tiles: PRICE, VS SPX, 10-YEAR, SECTOR FACTOR — current + prior close.
4. FROM YESTERDAY — one print, one lesson.
5. WHY IT IS ON THE TAPE — one job-site sentence.
6. EVENT — earnings / CPI / FOMC / housing / headline / none. Table, not a paragraph.
7. SCRIPT — band + tilt + why the overnight tape moved.
8. 10k PATHS — recipe, four tiles (MEAN, BAND, P(GREEN)/P(BEATS SPX), OUTSIDE), veto line. Stamp written before the sim.
9. BOOK — sleeve, stamp, kill. Cash leftover listed.
10. BEST TICKET last — one table, stamps only.

## 10k GATE — 9:10 · DO NOT LOCK WITHOUT THIS
1. ES, 10-year (bp), WTI, copper printed with time.
2. Width source marked: IV or 20-day realized.
3. Betas written or marked ZERO.
4. Event flag written or NONE.
5. Stamp sentence exists above the sim.
6. Veto math run. |μ| < 0.35 σ → PASS.
7. $10k book does not use a name that is PASS.

## Upload checklist
- [ ] Live filename is the canonical name, not `(1)`.
- [ ] Page is one HTML file. No iframe.
- [ ] Only one header.
- [ ] All ten sections present with real notes, not placeholders.
- [ ] Ledger row count did not shrink.
- [ ] After push, open the live URL and confirm the long version.

## Do not
- Redirect `index.html` to a stub.
- Wrap a dive in an iframe to add a header.
- Overwrite a real dive with a 2kb stub.
- Lock the book while the 9:10 factor row is missing.
- Let P(GREEN) create a ticket the sentence did not already stamp.
