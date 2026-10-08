# WP Agent orchestration skill

Public, source-only snapshot of the author's WP skill used as design evidence for [ultra-build](https://github.com/zenenznze/ultra-build). Pinned source commit: `c838d3e02220e0327229cd74bde0f931f49082ae`. No private Git history or task records are included. The synthetic privacy-scanner fixture uses `/home/demo/`.

WP provides durable HANDOFF contracts, bounded delegation/recovery, review and Herdr resource tracking. This is a reference snapshot, not a claim that live Agent backends or paid integrations have been tested for public users.

## Installation and limits

Clone `https://github.com/zenenznze/skill-wp-reference.git` and expose its root `SKILL.md` in your Agent client's skill directory. The skill expects an external `asm` freshness gate, `dev` delivery skill, Herdr, Pi and suitable Agent backends; these are not bundled. Read `SKILL.md` before operational use. Optional Jev integration needs separately authorized credentials and can incur cost; no live integration is invoked by this release.

The TypeScript control plane uses `npm ci` and `npm run build`; runtime Pi/Herdr peer dependencies must be supplied by the host. See `package.json`, `references/protocol.md` and `references/durable-supervisor.md`. Do not run unknown task commands or publish worker output without independent acceptance.

## License and attribution

Author-owned code is MIT licensed. **Adapted code**, not merely inspiration: four files derive from [ythx-101/agent-sop](https://github.com/ythx-101/agent-sop), MIT, copyright 2026 ythx-101. Exact file mappings and the complete upstream license are retained in `NOTICE.md` and must travel with redistributed copies. Other Agent clients and services are external integrations, not bundled implementations.
