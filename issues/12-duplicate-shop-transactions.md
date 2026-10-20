# Issue #12: Duplicate shop transactions during testing

**Status:** OPEN  
**Labels:** bug, economy  
**Opened by:** ByteMiner on 2026-10-07

## Description
In the Season 5 test world, one shop purchase occasionally generates two transaction records after a delayed acknowledgment. No production impact has been observed.

**Expected:** one purchase → one record.
**Actual:** intermittent duplicate in synthetic test ledger.

See `docs/economy-test-plan.md`.

## Discussion

### RedstoneRanger — 2026-10-07
> Thanks for reproducing this. Please keep the test-world revision and timing in the notes. No live rollout until we understand it.

### ByteMiner — 2026-10-09
> The duplicate seems tied to retry handling. I have a revised approach but need to rerun the full transaction checks.

### RedstoneRanger — 2026-10-17
> Still open after the technical review. Jordan, please attach the new test results before I approve the configuration.
