# CianOS / LifeOS — Self-Improvement RPG

> **Status: browser-based MVP/prototype — not a verified cloud platform.**

[Live demo](https://cianium.github.io/Self-Improvement/) · [Repository](https://github.com/cianium/Self-Improvement)

CianOS explores a game-inspired approach to personal development: personal goals become quests, practice earns experience points, and habits and language-learning activities are represented as progression systems.

## Current source

The repository contains a static HTML/CSS/JavaScript interface and separate state, routing and feature modules. It explores:

- Character dashboard, skills and rank/XP progression
- Daily missions and quest UI
- Inventory and rewards concepts
- Learning/vocabulary sections and personal progress views

**Note:** available features are prototype UI/logic; the presence of a screen is not evidence of secure account sync, production AI or verified learning outcomes.

## Run

```bash
git clone https://github.com/cianium/Self-Improvement.git
cd Self-Improvement
python3 -m http.server 8080
```

Open `http://localhost:8080`. Use a local server rather than assuming every ES-module feature works from `file://`.

## Repository map

- `index.html` — application shell
- `css/` — layout and theme
- `js/app.js`, `js/router.js`, `js/state.js` — app bootstrap, navigation and state
- `js/modules/` — features
- [Roadmap](ROADMAP.md) · [Changelog](CHANGELOG.md) · [Contributing](CONTRIBUTING.md)

## Versioning and next steps

GitHub Releases include `v1.3`; older documentation used `CianOS V2` and code comments refer to V3. Align marketing labels with actual release tags before advertising a numbered product release.

Next priorities: explicit persistence contract, test coverage, accessibility checks, user export/delete flows and measurable acceptance criteria for any future AI features.

## License

See [LICENSE](LICENSE) for current repository terms. Do not assume third-party assets are covered by that license.
