# bee-hive-oss

bee-hive-oss is the public home for open-source work by Bee. The aim is a layer of trust between humans and AI teams. Code built with AI should be open, so the work comes here when it is ready for anyone to use and inspect.

Private repositories move into this organization only when Bee says they go public.

The work here is credited to Bee, Grok Bot, and Nori together. The GNU tool ports are licensed under GPL-3.0-or-later.

## Public now

- [cursor-private-git](https://github.com/bee-hive-oss/cursor-private-git) helps you run Cursor cloud agents against a self-hosted Forgejo server, through Cloudflare Tunnel and Access.

- [ed-rs](https://github.com/bee-hive-oss/ed-rs) is a clean-room Rust port of GNU ed. It passes all 243 checks of the official GNU ed 1.22.4 test suite, plus the 20 starter cases byte for byte against GNU ed, with `cargo test` and `cargo clippy -D warnings` clean. Code coverage is measured on GitHub Actions with the GNU test suite only: C 84.2% lines / 67.4% branches, Rust 79.7% / 66.2%. The Rust port trails the C slightly.

- [patch-rs](https://github.com/bee-hive-oss/patch-rs) is a Rust port of GNU patch 2.8. It currently passes 44/49 of the official GNU patch test suite. Coverage on that same suite, also measured on GitHub Actions: C `src/` 76.4% lines / 65.3% branches, Rust 81.6% / 70.2%. The Rust port already exceeds the C. [PR #22](https://github.com/bee-hive-oss/patch-rs/pull/22) rejects absolute out-of-tree creates on reverse delete (CVE-2026-115207 / GNU patch 2.8).

Each port keeps a SCOREBOARD.md that updates automatically on every merge. Coverage columns are included from now on.

## In progress / coming soon

- Next GNU ports, underway: sed, grep, gawk, m4, bc, gzip, cpio, tar, and make.
- Honeypot CI, an agent-safe CI that has to work with any locked-box setup you choose, through swappable connectors. It is not tied to one security box.
- Lockbox, the reference example of that locked box. It is meant to stand on its own. The parts share connectors so they can snap together, and you can swap in a block of your own if you want something different.
- bee-stack, a plugin of shared rules and skills for Grok Bot and Cursor, so your own bot teams and Cursor agents can work the way Bee works. It is also meant to stand on its own.
- A free, open-source codebase visualizer.

You should not have to adopt every piece to use one of them.

## About

Bee builds this in Plano, Texas, with help from AI teams. Read how it all fits together on the Cursor forum: [Project-001: the trust layer](https://forum.cursor.com/t/project-001-the-trust-layer/178844) and [Honeypot-CI/CD](https://forum.cursor.com/t/honeypot-ci-cd-the-future-of-dev-ops/178849).

## Support the work

Everything here is free. If it helps you, you can [buy Bee a pizza on Buy Me a Coffee](https://buymeacoffee.com/bee805) 🍕. It helps cover the cost of the tools used to build and maintain the work. Bee is also on [X](https://x.com/bee__805).
