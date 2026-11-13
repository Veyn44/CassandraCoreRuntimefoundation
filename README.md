# Cassandra Engine — Archived Core + Phase 2 Snapshot

This repository is a preserved reference snapshot of the Cassandra engine and its first integrated gameplay layer. It is archived for provenance, inspection and future Core reference; it is not the active development repository.

## Snapshot provenance

- **Source repository:** [Veyn44/NEW-GAME-CASS](https://github.com/Veyn44/NEW-GAME-CASS)
- **Source branch:** `main`
- **Exact source commit:** [`31c1cd4`](https://github.com/Veyn44/NEW-GAME-CASS/commit/31c1cd4bb5f4e9e85bfbb98b863903f57c1f518f)
- **Archive snapshot commit:** [`e94d8b5`](https://github.com/Veyn44/CassandraCoreRuntimefoundation/commit/e94d8b59b7e29599174c260baf1e7d989e61c051)

The archive was created from the integrated `NEW-GAME-CASS/main` state after Phase 2 had been merged. The original source commit and the archive snapshot are recorded above.

## What is preserved

- The reusable, domain-neutral Core runtime in [`src/core`](src/core/README.md).
- The Cassandra host runtime and Phase 2 gameplay integration.
- Unit identity and placement foundations, Dev Lab integration, Colony Leader Draft/locomotion, and persistence/save-load integration.
- The Phase 2 architecture, system contracts, acceptance record and test evidence.

Phase 2 was completed and user-accepted, then merged into the active repository's `main` on 2026-11-13. Its development branch `next-step/phase-2` was retained separately in the active repository pending a cleanup decision; this archive does not make that branch-management decision.

## Core boundary

Core owns generic runtime infrastructure. Cassandra host/gameplay systems own Unit/Pawn data, world/gameplay rules, presentation and host integration. No Core source changes were made as part of Phase 2.

Do not develop new gameplay features in this archive. Continue active work in [`Veyn44/NEW-GAME-CASS`](https://github.com/Veyn44/NEW-GAME-CASS). Any proposed Core change should be separately justified and reviewed against this preserved baseline.

## Documentation

The [documentation index](docs/README.md) links to the preserved architecture, Phase 2 plan, acceptance and testing records.

## Development and verification

Requires Node.js 20 or newer.

```sh
npm run test:core
npm run test:host
npm run test:all
```

The scripts are preserved with the snapshot. Their presence does not mean tests were re-run as part of this archival documentation update. Consult the Phase 2 test record for the historical CI and user-acceptance evidence.
