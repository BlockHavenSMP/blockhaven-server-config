# BlockHaven SMP — Season 5 Technical Readiness Plan

**Project:** The Ender Expansion  
**Owner:** Alex Morgan (`RedstoneRanger`)  
**Contributors:** Jordan Lee (`ByteMiner`), Taylor Chen (`ChunkLoader`), Sam Rivera (`OakGuardian`)  
**Status as of:** October 20, 2026 — In progress  
**Target launch:** November 7, 2026

> Fictional public project record for the BlockHaven cybersecurity education exercise. No operational secrets or production configuration are included.

## Objective

Prepare the Season 5 economy and shopping district without introducing transaction errors or unplanned downtime. The public launch date is November 7, but stability takes priority over adding features.

## Workstreams

| Workstream | Lead | Current state | Next checkpoint |
|---|---|---|---|
| Shop transaction behavior | Jordan | Duplicate-processing bug under investigation | Revised test configuration |
| Economy configuration review | Alex | Waiting for revised configuration | October 29 test deadline |
| Backup and rollback documentation | Jordan / Alex | Draft available | Review before deployment |
| Performance readiness | Taylor | Hosting alternatives under evaluation | October 27 comparison |
| Community messaging | Sam | Launch notice draft | After technical sign-off |

## Current testing notes

On October 7, Jordan reproduced a condition where a test shop transaction could be processed twice. The issue is tracked in the public `blockhaven-server-config` issue #12. The team has not yet confirmed a final fix. Do not describe this issue as resolved.

Alex will review the revised configuration after Jordan documents the test results. The review is a readiness check, not a commitment to deploy immediately.

## Dependencies and sequencing

1. Reproduce and isolate the transaction issue in the test environment.
2. Document the revised configuration and expected behavior.
3. Run repeatable tests before the October 29 checkpoint.
4. Confirm backups and a rollback procedure.
5. Decide whether hosting changes should be deferred until after launch.
6. Publish a final launch-readiness update.

**Coordination note (October 18):** Avoid testing an economy change and a hosting migration simultaneously. If performance work becomes urgent, schedule it as a separate change with a clear rollback path.

## Open questions

- Is the duplicate transaction behavior limited to the test configuration?
- What test evidence will be sufficient for Alex's sign-off?
- Will peak player activity during the Build-Off affect performance testing?
- Does Taylor's hosting recommendation change the launch sequence?

## Revision history

- **Sep 29:** Jordan opened economy migration tracking.
- **Oct 7:** Duplicate transaction behavior recorded.
- **Oct 16:** Alex requested coordinated planning across workstreams.
- **Oct 18:** Technical review added a change-sequencing note.
- **Oct 20:** Public status snapshot prepared.

## Related public resources

- [BlockHaven GitHub organization](https://github.com/BlockHavenSMP)
- [BlockHaven Discord](https://discord.gg/KFY7eDjg)
