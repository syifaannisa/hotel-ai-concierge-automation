# Security Policy

## Public repository policy

This repository must not contain:

- API keys or access tokens;
- Telegram bot tokens;
- OAuth client secrets or n8n credential metadata;
- personal Google Sheets identifiers;
- production webhook URLs;
- real guest names, email addresses, phone numbers, chat identifiers, or booking records.

All secrets should be stored in n8n credentials, environment variables, or an appropriate secrets manager.

## Before publishing changes

1. Export a clean workflow copy from n8n.
2. Remove credential metadata and production identifiers.
3. Replace sensitive values with environment-variable references.
4. Scan the repository for secrets.
5. Review screenshots and sample data for personal information.

## Reporting a security issue

Please do not open a public issue containing sensitive information. Contact the repository owner privately through the professional contact method listed on their portfolio.
