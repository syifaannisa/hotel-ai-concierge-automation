# GitHub Upload Guide — Version 3

## Important Mac note

Files beginning with a dot are hidden by default in Finder:

- `.gitignore`
- `.env.example`
- `.github`

Press:

```text
Command + Shift + .
```

to show or hide hidden files.

The earlier screenshot did not show `.gitignore` and `.env.example` because Finder hides dotfiles. They were not necessarily missing.

## Repository

Name:

```text
hotel-ai-concierge-automation
```

Description:

```text
A modular multi-channel hotel concierge automation built with n8n, Google Gemini, Telegram, Gmail, Tally, and Google Sheets.
```

Visibility:

```text
Public
```

## Upload sequence

### Batch 01 — Documentation foundation

Upload every item inside:

```text
01-documentation-foundation
```

Commit:

```text
docs: initialise project documentation and security policy
```

### Batch 02 — Website workflow

Commit:

```text
feat: add website and Tally guest intake workflow
```

### Batch 03 — Telegram workflow

Commit:

```text
feat: add Telegram concierge and booking state workflow
```

### Batch 04 — Email workflow

Commit:

```text
feat: add AI-assisted email concierge workflow
```

### Batch 05 — Technical documentation

Commit:

```text
docs: add architecture, schema, and testing references
```

### Batch 06 — GitHub maintenance

Commit:

```text
chore: add repository validation and contribution templates
```

## Before each commit

- Confirm that files appear at the repository root, not inside a batch-number folder.
- Confirm that no API key, bot token, spreadsheet ID, or personal data appears.
- Confirm that folder names remain lowercase.
- Confirm that `.gitignore`, `.env.example`, and `.github` are visible after using `Command + Shift + .`.

## After all batches

Add repository topics:

- `n8n`
- `ai-automation`
- `workflow-automation`
- `hotel-automation`
- `google-gemini`
- `telegram-bot`
- `gmail-automation`

Then pin the repository on your GitHub profile.
