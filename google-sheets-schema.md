# Google Sheets Schema

The workflows use one shared workbook with separate tabs. Tab names can be adjusted, but the corresponding n8n nodes must be updated.

## Recommended tabs

### Conversations

Stores normalised requests from the website and other general channels.

Suggested columns:

`timestamp`, `session_id`, `channel`, `guest_name`, `guest_phone`, `guest_email`, `guest_message`, `intent`, `language`, `urgency`, `ai_response`, `escalated`, `resolved`, `hotel_code`, `response_time_ms`

### Telegram_Sessions

Stores active conversation state.

Suggested columns:

`chat_id`, `step`, `guest_name`, `check-in`, `check-out`, `room_pref`, `guests`, `email`, `intent`, `last_update`

### Telegram_Log

Stores Telegram interaction history.

Suggested columns:

`timestamp`, `chat_id`, `guest_name`, `message`, `reply`, `intent`, `status`

### Email_Log

Stores email enquiry and response history.

Suggested columns:

`Timestamp`, `Channel`, `Guest Name`, `Guest Email`, `Subject`, `Guest Message`, `AI Reply`, `Intent`, `Language`, `Status`

## Production note

Google Sheets is appropriate for a transparent portfolio demonstration and limited-volume prototypes. For production workloads, use a database with access control, validation, retention rules, auditability, and appropriate privacy safeguards.
