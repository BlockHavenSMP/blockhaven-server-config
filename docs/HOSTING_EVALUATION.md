# BlockHaven SMP — Hosting and Performance Evaluation

**Prepared by:** Taylor Chen (`ChunkLoader`)  
**Reviewers:** Alex Morgan (`RedstoneRanger`), Jordan Lee (`ByteMiner`)  
**Snapshot:** October 20, 2026  
**Comparison due:** October 27, 2026  
**Status:** Draft — no migration decision made

> Fictional educational document. Figures below are illustrative observations, not actual benchmark results or vendor claims.

## Why this review exists

BlockHaven players have reported intermittent lag during busy sessions since September 18. Performance appears to deteriorate around 25–30 concurrent players. The upcoming Build-Off may increase activity before Season 5.

## Questions to answer

- Is the main bottleneck CPU scheduling, plugins, world activity, or hosting capacity?
- Would targeted optimization help without a host migration?
- How much operational risk would a migration introduce before November 7?

## Preliminary observations

| Observation | Current understanding | Confidence |
|---|---|---|
| Tick-rate drops during peak play | Repeatedly reported by players | Medium |
| Peak activity near 25–30 players | Correlates with worst reports | Medium |
| Plugin overhead | Possible contributing factor | Low |
| Hosting capacity | Not yet isolated as the cause | Low |

## Options under review

### A. Stay on the current host and optimize

Lowest disruption. Investigate plugin overhead and world activity first. May not fully resolve capacity limitations.

### B. Upgrade the current hosting plan

Potentially simpler than migration, but requires confirming that the relevant bottleneck is actually addressed.

### C. Migrate to a different host

Could offer better performance, but introduces data-transfer, DNS, rollback, and scheduling work. Not preferred immediately before launch without stronger evidence.

## Decision criteria

| Criterion | Weight in discussion |
|---|---|
| Measured improvement under realistic load | High |
| Reliable backup and restore process | High |
| Change risk before Season 5 | High |
| Ongoing cost | Medium |
| Staff time required | Medium |

## Coordination notes

- **Oct 10 — Taylor:** Collect additional observations before comparing providers.
- **Oct 11 — Jordan:** Check plugin overhead so a host migration does not mask the underlying issue.
- **Oct 17 — Taylor:** Comparison draft expected October 27.
- **Oct 18 — Alex:** Avoid changing infrastructure while economy testing is still unresolved unless evidence clearly justifies it.

## Next steps

1. Gather a repeatable sample of performance observations.
2. Complete a comparison of optimization, plan upgrade, and migration.
3. Present recommendations to Alex by October 27.
4. Coordinate any approved change with economy testing and the November 7 launch.

## Revision history

- **Sep 18:** Initial performance investigation began.
- **Oct 10:** Hosting alternatives added to review.
- **Oct 17:** Comparison deadline confirmed.
- **Oct 20:** Public draft snapshot issued.
