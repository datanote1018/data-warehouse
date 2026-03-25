# Contributing Guide

Thanks for your interest in contributing! This guide keeps things simple — just a few rules to keep the project consistent.

---

## Branch Rules

- **`master` is protected.** No direct pushes — all changes go through Pull Requests.
- Create your branch from `master`, name it clearly:
  - `add/glossary-trade` — new content
  - `fix/sql-tutorial-typo` — bug fix
  - `update/standards-naming` — update existing content
- Each PR requires **at least 1 review** before merging.
- Use **Squash and Merge** to keep commit history clean.

## Directory Structure

```
data-warehouse/
├── index.html              ← Site homepage (update when adding new modules)
├── assets/style.css        ← Shared styles (do not duplicate in subfolders)
├── sql-tutorial/           ← SQL practice platform
├── standards/              ← DW standards and guidelines
├── glossary/               ← Naming word roots
└── docs/                   ← Project documentation (not user-facing content)
```

## Naming Conventions

| Item | Rule | Example |
|------|------|---------|
| Directory | lowercase, hyphen-separated | `sql-tutorial/` |
| HTML file | lowercase, underscore for multi-word | `sql_practice.html` |
| CSS/JS | lowercase, hyphen-separated | `style.css` |
| Branch | `type/short-description` | `add/glossary-finance` |

## Adding New Content

1. **Open an Issue first** — briefly describe what you want to add, so maintainers can align with you before you start coding.
2. Create the directory if it doesn't exist.
3. Your HTML file must reference the shared stylesheet:
   ```html
   <link rel="stylesheet" href="../assets/style.css">
   ```
4. Follow the dark theme and color variables defined in `assets/style.css`. See [Style Guide](docs/style-guide.md) for details.
5. Update `index.html` to add an entry card for the new module.
6. Submit a PR using the PR template.

## Commit Messages

Keep it short and clear. Use a prefix:

```
add: sql tutorial exercise for window functions
fix: broken link in glossary page
update: standards naming convention section
docs: improve contributing guide
```

## What We Review

Before approving a PR, reviewers check:

- [ ] Branch is based on latest `master`
- [ ] Content is accurate and clearly written
- [ ] HTML follows the shared style (dark theme, consistent layout)
- [ ] No broken links or missing assets
- [ ] `index.html` updated if a new module was added
- [ ] Commit messages are clean

## Questions?

Open an Issue with the **Question** label, or start a Discussion. We're happy to help!
