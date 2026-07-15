# Sanitisation Verification Report

The repository package was scanned for the known sensitive values present in the original exports.

## Checks performed

- hard-coded Gemini API keys;
- hard-coded Telegram bot tokens;
- the original Google Sheets identifier;
- n8n `credentials` metadata blocks;
- cached Google Sheets result URLs;
- workflow-level webhook identifiers.

## Result

No known sensitive values were detected in the sanitised workflow files.

## Important limitation

Automated scanning reduces risk but does not guarantee that every possible sensitive value has been identified. Review the files manually before making the repository public, and rotate any token or API key that appeared in the original exports.
