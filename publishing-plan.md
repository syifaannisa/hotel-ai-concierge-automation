# GitHub Publishing Plan

Publish the repository in several meaningful commits rather than one unexplained upload.

## Recommended sequence

### Commit 1

```text
docs: initialise project documentation and security policy
```

Upload:

- `README.md`
- `LICENSE`
- `SECURITY.md`
- `.gitignore`
- `.env.example`
- `docs/`
- `assets/project-cover.svg`

### Commit 2

```text
feat: add website and Tally guest intake workflow
```

Upload:

- `workflows/website-tally-concierge.json`

### Commit 3

```text
feat: add Telegram concierge and booking state workflow
```

Upload:

- `workflows/telegram-concierge.json`

### Commit 4

```text
feat: add AI-assisted email concierge workflow
```

Upload:

- `workflows/email-concierge.json`

### Commit 5

```text
docs: add architecture, schema, and testing references
```

Upload any remaining documentation and sample schema.

### Commit 6

```text
chore: add repository validation workflows and contribution templates
```

Upload:

- `.github/`
- `CONTRIBUTING.md`
- `CODE_OF_CONDUCT.md`
- `CHANGELOG.md`

### Commit 7, after screenshots are ready

```text
docs: add workflow screenshots and guest journey demo
```

## Release

After final review, create:

```text
v1.0.0 — Portfolio Demonstration Release
```

Do not create artificial commits solely to increase the commit count. Each commit should represent a real, reviewable improvement.
