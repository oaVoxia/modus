# Modus

*Est modus in rebus.* There is a proper measure in things.

Modus shows which feature, customer, and model left the measure on your LLM bill. It is a cost ledger and a morning review. It is not a proxy, not a prompt store, and not a FinOps suite.

Provider invoices arrive as one number, or a split by API key. Keys are shared, so a chat feature, an embeddings backfill, and a forgotten eval job look the same. Modus attributes spend to the names you already use in code, then marks the day something breaks its pattern.

## Who it is for

The engineer who owns the model bill, usually at a seed to Series B company spending roughly $500 to $30k a month across more than one provider. Finance reads the monthly account. Finance does not set the product up.

## Principles

1. **Measure, don't seize.** Observe and mark. v1 never blocks a request.
2. **Take nothing you do not need.** Metadata only: model, token counts, latency, tags, estimated cost. No prompts, no completions.
3. **What is uncounted is not governed.** Untagged spend is first-class and called *sine nomine*.
4. **The account is the product.** The dashboard is a reference. The morning letter is what people come back for.

## The four artifacts

| Name | What it is |
| --- | --- |
| **The measure** | A monthly dollar limit on the workspace, and optional limits per feature. |
| **A nota** | A mark when a slice of spend leaves its pattern. Grades: nota, censura, ignominia. Fixed thresholds, not a model. |
| **The examen** | A morning letter. Three numbers, one cause, one act. |
| **The rationes** | A monthly export for finance: spend by feature, model, and customer, plus the marks that fired. |

## How spend gets in

The SDK is the default. The app calls the provider as it does today, then reports token counts to Modus. Modus is not on the critical path.

A proxy that swaps the base URL is an on-ramp only. It is not the product. Holding a provider key is a liability.

Every dollar in the UI is estimated from a price book. Teams can pin a rate when a lab changes prices.

## What v1 refuses

- Prompt or completion storage
- Model routing, caching, and retries
- Anomaly detection by model
- Stripe revenue join
- Blocking or downgrading a request when the budget breaks

## Status

Private. Not built yet. The charter above is the spec until code replaces it.
