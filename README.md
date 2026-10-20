# BlockHaven SMP — Server Configuration Notes

> BlockHaven SMP is a fictional Minecraft community created for an authorized OSINT training event. All examples are synthetic; no production access, secrets, or real server infrastructure are provided.

Public-facing notes and *illustrative* configuration samples for BlockHaven SMP Season 4 → Season 5. These files are not deployed configurations and are not guaranteed to be accepted by any specific Minecraft plugin.

**Maintainers:** Alex Morgan (`RedstoneRanger`, lead administrator), Jordan Lee (`ByteMiner`, plugin development), Taylor Chen (`ChunkLoader`, infrastructure).

## Current priorities (as of October 20, 2026)
- **Season 5 — The Ender Expansion:** target launch **November 7, 2026**.
- **Economy migration:** target validation complete **October 29**; transaction duplication under investigation in [issue #12](issues/12-duplicate-shop-transactions.md).
- **Performance:** peak-hour tick-rate drops with roughly 25–30 players; see [issue #17](issues/17-peak-hour-performance.md).
- **Hosting review:** Taylor's options comparison due **October 27**; no production migration approved.

## Repository map
- [`docs/season5-plan.md`](docs/season5-plan.md) — roadmap and sequencing.
- [`docs/economy-test-plan.md`](docs/economy-test-plan.md) — reproduction steps and acceptance checks.
- [`docs/hosting-review.md`](docs/hosting-review.md) — performance and hosting considerations.
- [`docs/rollback-checklist.md`](docs/rollback-checklist.md) — non-sensitive rollback policy.
- [`config/economy.sample.yml`](config/economy.sample.yml) — synthetic, non-executable settings illustration.
- [`data/performance-observations.csv`](data/performance-observations.csv) — invented metrics for discussion.
- [`issues/`](issues/) — issue discussions mirrored as Markdown for read-only browsing.

For official updates, see the BlockHaven website's News and Changelog pages.

**Contact:** Alex Morgan — alex.blockhaven@gmail.com
