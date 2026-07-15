# Setup Guide

## Prerequisites

- an n8n instance;
- a Google account with Gmail and Google Sheets access;
- a Telegram bot;
- a Google Gemini API key;
- a Tally form or equivalent website form;
- a shared Google Sheets workbook using the documented tab structure.

## 1. Configure secrets

Copy `.env.example` to your private environment configuration and add the required values.

Do not commit `.env` or secret values to GitHub.

## 2. Configure n8n credentials

Create credentials through the n8n credential manager:

- Gmail OAuth2;
- Google Sheets OAuth2.

The public workflow files intentionally contain no credential metadata. Select the correct credential manually after import.

## 3. Import the workflows

Import each JSON file from the `workflows` folder into n8n.

After importing:

1. open every node showing a configuration warning;
2. select the appropriate credential;
3. confirm the Google Sheet and tab names;
4. configure trigger or webhook URLs;
5. test each workflow with sample data before activation.

## 4. Telegram workflow

- create a bot through Telegram BotFather;
- store the token in `TELEGRAM_BOT_TOKEN`;
- configure Telegram to send updates to the n8n webhook;
- verify that the session and log tabs exist.

## 5. Email workflow

- connect Gmail through OAuth2;
- confirm the inbox filter;
- set the Google Sheet destination;
- test with a non-sensitive demonstration email.

## 6. Website and Tally workflow

- connect the Tally form webhook to the n8n webhook;
- confirm that form labels match the labels expected by the normalisation node;
- replace simulated PMS behaviour with a real integration only after authentication, validation, and error handling are implemented.

## 7. Validation checklist

- no secret is visible in a node URL or request body;
- no real guest data is used;
- every workflow returns a controlled error or fallback response;
- logs are written to the intended sheet;
- language, intent, booking, and escalation paths are tested separately.
