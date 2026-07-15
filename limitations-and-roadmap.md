# Limitations and Roadmap

## Current limitations

- This repository is a demonstration project, not a production hotel system.
- Google Sheets is used as a lightweight shared data layer.
- PMS behaviour is simulated or incomplete.
- Availability and booking confirmation should not be treated as authoritative without a real PMS.
- Error handling, retries, monitoring, rate limiting, and idempotency require further production hardening.
- Guest authentication and privacy controls are not fully implemented.
- SMS and WhatsApp channels are not currently included as operational workflows.
- AI-generated replies should use human escalation rules for sensitive, urgent, payment, safety, or complaint-related cases.

## Planned improvements

1. Integrate a production PMS or reservation API.
2. Add Twilio SMS and WhatsApp Cloud API channels.
3. Replace Google Sheets session state with a database.
4. Add structured observability, execution alerts, and retry policies.
5. Add approval gates for complaints, refunds, payment requests, and high-urgency messages.
6. Add automated tests with representative multilingual payloads.
7. Add data-retention and privacy controls.
8. Add analytics for enquiry volume, intent distribution, response time, and escalation rate.
