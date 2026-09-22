# TAPE STANDARD

Purpose: read the whole tape, post only live numbers, stamp before the sim, get smarter after every close.

Applies to OPEN, every ticker card, the $10k book, and the ledger. No exceptions.

This is a desk notebook. Not advice. Not a broker. Not a signal service.

## WORKING NAME
THE TAPE
Sister desk to THE SPLIT. Same stamps. Same lock discipline. Same ledger religion.

## LEDGER LOCK
`tape-ledger.json` is the record. SETTLED rows never leave.
- Read the live file first. Count `tickets`.
- Patch by `id` or APPEND a new `id`. Never write fewer `tickets` than you read.
- Forbidden: `tickets: []`, PLACEHOLDER, a one-row stub, rebuilding from memory.
- "No OPEN tickets" is not an empty ledger. Cash is a legal position.
- If a write would truncate the JSON, skip `tape-ledger.json` that pass.

Two books, two files. Do not mix.
- `tracker.json` = sports
- `tape-ledger.json` = tape

## HOURS
Day = America/New_York.
- Premarket read: 7:00
- LOCK (T-20): 9:10
- Open: 9:30
- Closeout: 16:00
- Grade: 16:15 same day
No OPEN ticket survives the close. Flat or SETTLED by 16:15.

## Watchlist v1
CAT DE URI VMC MLM HD LOW LEN DHI XOM CVX UNP VOO IEF

## CONFIDENCE
Stamp before the 10k. Sim may only veto. P(GREEN) is never a second reason.
BET / LEAN / FADE / PASS. PASS is the common stamp. A one-day stock BET is almost never legal.

Veto: |mu| < 0.35 * sigma_day -> PASS.

## TWO ENGINES
- 10k PATHS = 10,000 session draws
- $10k BOOK = paper bankroll. Max two leans. Max $2,000 sleeve. Cash is legal. No leverage. No options. No shorts in v1.

## KILLS
1. 10-year reverses the overnight move by 9:45 -> rates leans dead
2. ES gives back the whole overnight move by 10:30 -> beta leans dead
3. Company headline -> that name dead
4. Halt -> that name dead

## UPDATE COMMAND
When the user says tape update: lock tape-ledger.json first, close yesterday, board today, push CJD0314/the-tape main.

Full spec lives in the working copy of TAPE-STANDARD in the first commit notes and in the conversation desk rules. Expand this file on the next tape update if any rule is missing from this short board copy.
