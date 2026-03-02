# CLAUDE.md — AI Assistant Guide for A5HW1NR/A5HW1NR

## Repository Overview

This is **Ashwin Ramesh's GitHub profile repository** (`A5HW1NR/A5HW1NR`). GitHub renders the `README.md` of a repository that matches the username as the profile homepage at `github.com/A5HW1NR`.

**Single file. No build system. No tests. No dependencies.**

---

## Repository Structure

```
A5HW1NR/
└── README.md    # GitHub profile page — the entire codebase
```

### README.md Contents

The file has two distinct sections:

1. **Profile intro** (lines 1–29): Bio, skills, GitHub stats badge, learning goals, and contact links.
2. **Interactive text adventure game** (lines 31–134): "Escape the Office" — a Markdown-based choose-your-own-adventure game using anchor links (`#section-id`) to simulate navigation between scenes.

---

## Owner Profile

- **Name:** Ashwin Ramesh
- **Role:** Security engineer & researcher
- **Languages:** Python, Go, HTML, CSS, React
- **Databases:** SQL, PostgreSQL, DynamoDB
- **Cloud:** AWS, GCP
- **Data science:** Pandas, NumPy
- **Contact:** ashwin94.ramesh@gmail.com | [LinkedIn](https://www.linkedin.com/in/a5hw1n/) | [Twitter/@AshwinRamesh94](https://x.com/AshwinRamesh94)

---

## Development Conventions

### Markdown Style
- Use `##` for top-level sections, `###` for sub-sections.
- HTML anchor tags (`<h2 id="...">`) are used for game navigation targets — this is intentional and required for the choose-your-own-adventure mechanic.
- GitHub-flavored Markdown (GFM) is the rendering target.
- Emoji are used throughout — preserve them when editing existing sections.

### GitHub Stats Badge
The stats badge at line 16 uses the `github-readme-stats` Vercel service:
```
https://github-readme-stats.vercel.app/api?username=A5HW1NR&show_icons=true&theme=radical
```
Update `username=` if the GitHub handle ever changes.

### Interactive Game Structure
The game uses intra-page anchor links. Each scene is an `<h2 id="...">` block followed by choices as Markdown links. Valid scene IDs:
- `escape-the-office` — start/restart
- `copier`
- `desk`
- `exit`
- `server-room`
- `do_not_opentxt`
- `delete`
- `trap` (game over)
- `freedom` (win)
- `caught` (game over)

When adding new scenes, follow the same `<h2 id="scene-name">` + `---` divider pattern.

---

## Git Workflow

- **Default branch:** `master`
- **No CI/CD, no linters, no pre-commit hooks**
- Commit messages have been simple and descriptive (e.g., "Update README.md", "md interactive game")
- All changes go directly to `master` for a profile repository

### Making Changes
1. Edit `README.md` directly — it is the only file that matters.
2. Commit with a clear message describing what changed.
3. Push to `master`.

```bash
git add README.md
git commit -m "Brief description of change"
git push origin master
```

---

## What AI Assistants Should Know

- **Do not add files beyond README.md and CLAUDE.md** unless explicitly asked. A profile repo should stay minimal.
- **Do not add a build system, package manager, or tests** — there is nothing to build or test.
- **Preserve existing anchor IDs** in the game section; breaking them breaks the game navigation.
- **The GitHub stats badge URL is external** — do not treat it as broken even if it doesn't resolve locally.
- **Emoji are intentional** — do not strip them during edits.
- When updating the profile section, maintain the existing heading hierarchy and section order.
