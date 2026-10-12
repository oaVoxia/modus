# Modus

*Est modus in rebus.* There is a proper measure in things.

Modus shows which feature, customer, and model left the measure on an LLM bill. The lite build is a ledger and a morning review. It is not a proxy, and it does not store prompts.

## Lite build

Northwind is a sample ledger, closed through 11 Oct 2026. Yesterday includes a backfill that had been silent for a week. The month projects past a $6,000 measure until you raise it.

| Surface | What it does |
| --- | --- |
| Today | Yesterday, pace, sine nomine, the examen |
| Features | Spend, requests, top model, week-over-week |
| Customers | Who the tagged spend belongs to |
| Nota | Marks. Accept a nota or a censura. Ignominia clears only when the projection sits inside the measure |
| Measure | The monthly number, kept in this browser |
| Install | `POST /api/ingest` prices a call. A test call shows up as live spend and does not rewrite yesterday |

Sending `prompt`, `completion`, or `messages` returns 400.

Dollars are estimates from a small price book, not an invoice.

## Cloudflare

The worker preset is `cloudflare-module`, with `nodejs_compat`, and the Worker name is `modus`. `wrangler.json` in the project root is merged into the generated worker config at `.output/server/wrangler.json`.

Ingest uses the Web `Request` / `Response` APIs only. It does not touch the filesystem or a database. Live calls stay in the browser.

The default production build stays on the Vercel preset so the hosted preview keeps working. Set `NITRO_PRESET=cloudflare` to emit the Worker.

## Still out of this lite build

- No provider keys, and no request proxy
- No mailed examen
- No pinned rates
- No server-side history
