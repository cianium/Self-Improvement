# CianOS — Release history and version policy

> **Maintainer audit: 2026-10-26.** This file describes what GitHub currently publishes. It does **not** rewrite or create releases, tags, or binary assets.

## Published GitHub releases

| Tag | GitHub classification | Published (UTC) | Commit | Source difference |
| --- | --- | --- | --- | --- |
| [v1.0](https://github.com/cianium/Self-Improvement/releases/tag/v1.0) | Release | 2026-10-18 02:14 | `5ef0b265040ecf1335e5a4d4e5dc70e67ac8b8b7` | Identical to the other two tags |
| [v1.2](https://github.com/cianium/Self-Improvement/releases/tag/v1.2) | Pre-release | 2026-10-18 02:16 | `5ef0b265040ecf1335e5a4d4e5dc70e67ac8b8b7` | Identical to the other two tags |
| [v1.3](https://github.com/cianium/Self-Improvement/releases/tag/v1.3) | Release | 2026-10-18 02:17 | `5ef0b265040ecf1335e5a4d4e5dc70e67ac8b8b7` | Identical to the other two tags |

**Critical provenance detail:** GitHub's compare API reports **0 commits and 0 changed files** between `v1.0` and `v1.3`. Therefore the tags are **three historical labels for the same Git source snapshot**; they are not proof of three sequential feature releases.

Each GitHub release description links to a separately uploaded ZIP under `github.com/user-attachments/`, not an actual asset attached to that release. These ZIPs were not inspected in this audit. Their filenames (`UrOS-main.zip`, `level-up-yourself-main.zip`, `Self-Improvement-main.zip`) may refer to different files, but differences **cannot be inferred from the tags**. GitHub reports zero release assets for the three entries.

## Name and version clarification

- **CianOS** is the product name used in this repository.
- **Life RPG** describes the product concept; `Self-Improvement` is the GitHub repository name.
- Current HTML and source comments contain **`CianOS Ultra V3`**.
- The historic `CHANGELOG.md` entry says **`2.0.0`**, but there is **no verified corresponding `v2.0.0` tag** in the published releases checked here.
- **`v1.3` is the most recent published GitHub release**, not necessarily the version of the latest `main` README or the conceptual V3 development UI.

Do not describe V2/V3 source labels as new GitHub releases without creating verified tags from tested commits.

## Draft text for each existing release

These sections are suggested replacements for GitHub's current sparse release descriptions. **They have not been applied to the GitHub Releases UI.**

### v1.0 — Historical CianOS snapshot

> Historical published label for the browser-based CianOS Life RPG prototype. The `v1.0`, `v1.2` and `v1.3` Git tags currently reference the same source commit, so distinct functionality for this label cannot be verified from Git history. This project uses HTML, CSS and vanilla JavaScript. Not a production cloud service. ZIP attachment linked in the original release description was not independently inspected.

### v1.2 — Historical preview label

> Historical pre-release label. This tag points to the same Git commit as `v1.0` and `v1.3`; it does not document a separately verifiable code revision. The earlier user-uploaded ZIP may differ, but its contents have not been audited. Keep the pre-release marker for historical accuracy unless the original artifacts are reviewed.

### v1.3 — Latest published GitHub release label

> Most recently published GitHub release for CianOS, a browser-based Life RPG prototype with RPG-themed character/XP, quest, learning and progression UI. The `v1.3` tag points to the same snapshot as `v1.0` and `v1.2`; it should not be interpreted as evidence of additional features compared with those two tags. The active `main` branch contains subsequent documentation changes only (as of this audit). No production backend, cloud account sync or live AI service has been verified.

## Policy for future releases

1. Create a **new tag only from a tested, identified commit**. Never move published tags silently.
2. Record a changelog describing *actual source changes* since the previous unique commit.
3. Use a clear release title such as `CianOS vX.Y.Z — <short milestone>`.
4. Mark preview builds as GitHub **Pre-release**; reserve **Latest** for a genuinely tested non-preview release.
5. Attach any distributable ZIP to the GitHub release's **Assets**, rather than linking only to an unrelated upload in its description.
6. Confirm that the ZIP source matches the tagged commit and list a checksum when practical.
7. Note client-side `localStorage` limitations, missing account sync, and the absence of server-side AI or financial integrations.
8. Keep screenshots and any third-party media lawful and clearly credited.

## Next administrative action

Using GitHub's **Releases → Edit**, change the three titles and bodies to the suggested wording above, **without deleting or retargeting their tags**. Direct editing of release metadata is not provided by the current connected GitHub toolset.
