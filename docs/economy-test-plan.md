# Economy migration — test notes

Maintainer: Jordan Lee (`ByteMiner`)  
Review required: Alex Morgan (`RedstoneRanger`)

## Observed issue
On October 7, 2026, a test-world shop purchase occasionally appeared twice in the transaction ledger when a retry coincided with a delayed acknowledgment. This is a *fictional* behavior in a simulated plugin integration, not a vulnerability report for a real product.

## Reproduction outline (simulated)
1. Use a test-only world and synthetic player balances.
2. Initiate a single shop purchase with simulated delayed acknowledgment.
3. Compare the visible purchase count with the recorded transaction count.
4. Record revision, timing, and whether the duplicate is reproducible.

## Acceptance criteria
- One purchase produces one ledger record.
- Repeated test runs preserve balance consistency.
- A rollback plan is documented before any live change.
- Jordan provides test notes; Alex approves the release decision.

**Target:** October 29, 2026. See issue #12 and #14.
