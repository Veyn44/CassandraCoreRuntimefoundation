# Archived Project Documentation

This documentation describes the preserved Core + Phase 2 snapshot from `NEW-GAME-CASS/main` at commit [`31c1cd4`](https://github.com/Veyn44/NEW-GAME-CASS/commit/31c1cd4bb5f4e9e85bfbb98b863903f57c1f518f).

This repository is a reference archive, not the active development target. Current gameplay planning and future implementation belong in [`Veyn44/NEW-GAME-CASS`](https://github.com/Veyn44/NEW-GAME-CASS).

## Completed phase

- [Phase 2 — First Testable Game Layer](phases/PHASE_2.md) — completed, user-accepted and merged into the source repository's `main`.
- [Phase 2.4 — Persistence and Dev Lab Workspace](phases/PHASE_2_4_PERSISTENCE_PLAN.md) — final persistence contract, implementation notes and user acceptance.
- [Phase 2 test plan](testing/PHASE_2_TEST_PLAN.md) — automated and manual evidence, including explicit deferred checks.

## Architecture

- [Application Shell and Mode Architecture](architecture/APPLICATION_SHELL_AND_MODES.md) — application shell, Dev Lab/New Game separation and shared gameplay ownership.
- [Core Audit — Phase 2](architecture/CORE_AUDIT_PHASE_2.md) — source/API audit and the conclusions carried into the accepted Phase 2 implementation.
- [Phase 2 System Contracts](architecture/PHASE_2_SYSTEM_CONTRACTS.md) — host, Unit, Colony Control, locomotion and persistence contracts.
- [World Lifecycle](architecture/WORLD_LIFECYCLE.md) — approved persistent/temporary world model and its still-open implementation details.
- [Game Systems Architecture](architecture/GAME_SYSTEMS_ARCHITECTURE.md) — system ownership, dependencies and communication.
- [Repository Structure](architecture/REPOSITORY_STRUCTURE.md) — preserved directory layout and project boundaries.
- [World Geometry](architecture/WORLD_GEOMETRY.md) — world dimensions and coordinate conventions.

## Standards

- [System Development Standard](standards/SYSTEM_DEVELOPMENT_STANDARD.md) — system design, ownership, lifecycle, persistence and testing requirements.

## Archive rules

- Treat this repository as an immutable reference baseline.
- Do not continue Phase 2 development here; it has already been merged into the active repository.
- Do not interpret historical branch names or pre-merge checklists as current instructions. The final Phase 2 acceptance and merge records supersede them.
- Do not infer that a test passed merely because a test file or script exists. Use the recorded evidence and distinguish automated CI from user-confirmed browser checks.
- Do not modify Core casually. Any proposed Core change requires a concrete domain-neutral reason and a separate review.

A separate Phase 3 plan is intentionally not included in this archival snapshot. Refine future scope in the active repository when work resumes.
