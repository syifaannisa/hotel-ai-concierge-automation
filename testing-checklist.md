# Testing Checklist

## Website and Tally

- [ ] Valid booking request is normalised correctly.
- [ ] Missing email is handled safely.
- [ ] Missing optional dates do not break the workflow.
- [ ] Unknown form labels produce a controlled fallback.
- [ ] Duplicate webhook submission is identified or documented.
- [ ] Failed Google Sheets write is visible.

## Telegram

- [ ] `/start` displays the main menu.
- [ ] Booking flow stores each step.
- [ ] Existing session resumes correctly.
- [ ] Invalid guest count is handled.
- [ ] Invalid email input is handled.
- [ ] FAQ buttons return the expected answer.
- [ ] Room-service request is logged.
- [ ] Staff request is escalated.
- [ ] Completed booking closes or resets the session.
- [ ] Unknown callback data receives a safe response.

## Email

- [ ] New unread email triggers the workflow.
- [ ] Sender name and address are parsed.
- [ ] English message is classified.
- [ ] Italian or Albanian message is recognised.
- [ ] AI failure uses the fallback reply.
- [ ] Reply subject is formed correctly.
- [ ] Gmail send failure is visible.
- [ ] Interaction is logged.
- [ ] Complaint or urgent request is not treated as routine.

## Security

- [ ] No real guest data is used.
- [ ] No token appears in node URLs.
- [ ] No credential metadata is committed.
- [ ] No spreadsheet identifier is public.
- [ ] Screenshots hide browser addresses and account details.
