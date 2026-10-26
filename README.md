<div align="center">

# CianOS

### A browser-based Life RPG for personal growth and language learning

**Turn goals into quests, build streaks, and track progress through an RPG-inspired interface.**

[![Status](https://img.shields.io/badge/Status-Prototype-DAA520)](https://github.com/cianium/Self-Improvement)
![Stack](https://img.shields.io/badge/Stack-HTML%20%7C%20CSS%20%7C%20JavaScript-3178C6)
![License](https://img.shields.io/badge/License-All%20Rights%20Reserved-555555)

[Project demo](https://cianium.github.io/Self-Improvement/) · [Source code](https://github.com/cianium/Self-Improvement) · [Roadmap](ROADMAP.md) · [Changelog](CHANGELOG.md)

</div>

> **Project status:** CianOS is a client-side prototype, not a production account-based service. The linked GitHub Pages URL is a demo location, not proof of operational readiness. There is no verified backend, cloud synchronization, live AI mentor, or automated test pipeline in this repository.

## Overview

CianOS explores **gamified self-improvement** using the language of role-playing games: a character profile represents progress, quests model activities, experience points reward completed tasks, and learning activities can become part of a progression system.

The current codebase is a single-page website implemented in **vanilla JavaScript with ES modules**, HTML and CSS. It is designed as an experiment rather than a complete productivity or learning platform.

## Features in the source

| Module | What the source includes |
| :-- | :-- |
| **Character & progression** | Character statistics, level/XP indicators, ranks, currency and stat point allocation |
| **Quests** | Sample daily and side quest lists, completion actions and reward-related logic |
| **Skills & encounters** | Skill displays and game-like boss/encounter mechanics |
| **Vocabulary** | Lexicon UI with learning/mastered status and related interactions |
| **Streaks** | Date/streak display and tracking logic |
| **Inventory & economy** | Virtual gold/crystal balances and in-app item interactions |
| **Local persistence** | Browser `localStorage` read/write implementation through `StorageManager` |

**Important:** these are code-level features, **not independently verified end-to-end product flows**. The included quests, encounters, currencies and progress indicators are game mechanics, not prescribed physical activities, medical guidance, or real-money services.

### Not implemented or not verified

- User accounts, server-side authentication or multi-device synchronization
- Hosted databases, live AI recommendations or adaptive learning services
- Production analytics, backup/export guarantees or real purchase processing
- Automated CI, accessibility certification or comprehensive browser test coverage

Browser storage is device/browser-specific and can be cleared. Do not rely on it to preserve important personal records.

## Preview locally

You need a modern browser and a simple static HTTP server. No npm installation or framework build step is defined in the repository.

```bash
git clone https://github.com/cianium/Self-Improvement.git
cd Self-Improvement
python3 -m http.server 8080
```

Then open **http://localhost:8080**. Serving over HTTP is recommended because the application imports JavaScript ES modules.

## Repository structure

```text
index.html             App shell and screen markup
css/style.css          Visual design and responsive styles
js/app.js              App bootstrap and UI orchestration
js/router.js           Client-side view routing
js/state.js            Application state and sample content
js/utils/              Storage, XP and supporting helpers
js/modules/            Quests, streaks, vocabulary, skills, shop, encounters
ROADMAP.md             Planned development milestones
CHANGELOG.md           Historical release notes
CONTRIBUTING.md        Contribution guidelines
LICENSE                All-rights-reserved terms
```

## Versioning: source vs. published releases

Three different version references currently appear in the repository:

- **GitHub Releases:** the latest published tag found is `v1.3`.
- **Changelog:** documents a historical `2.0.0` / CianOS V2 milestone.
- **Current source comments and HTML title:** refer to **CianOS Ultra V3**.

These labels have **not been reconciled into one verified release sequence**. A source comment does not constitute a published `v3.0.0` release. This README intentionally uses the **CianOS** product name without claiming a validated current release version.

## Roadmap

The existing [roadmap](ROADMAP.md) sketches enhancements to progression, mobile experience, AI features, language-learning activities and a possible social ecosystem.

Recommended near-term engineering priorities:

1. Align source, changelog and release version names.
2. Validate that the modules work together and add automated UI and state tests.
3. Define browser-storage behavior, data export and reset options.
4. Improve keyboard accessibility, reduced-motion support and responsive behavior.
5. Treat AI integrations and hosted accounts as separate future milestones, not shipped functionality.

> **Documentation discrepancy:** `ROADMAP.md` still lists local persistence as a planned V3 feature, while `js/utils/storage.js` already implements browser `localStorage`. That implementation needs testing before the roadmap status can be updated confidently.

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md). Open an issue describing the proposed change before submitting a pull request.

## License

© 2026 Cian. **All rights reserved.** The repository's [LICENSE](LICENSE) does not grant permission to copy, modify, redistribute or commercially reuse the project without the owner's approval. Third-party fonts, icons or visual assets may have separate terms.

---

<div align="center">

**CianOS · Grow through small, meaningful progress.**

</div>
