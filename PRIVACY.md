# Kuyo Privacy Policy

Effective: August 7, 2026

Kuyo is a Discord bot that reads selected text messages aloud and gives short character replies when explicitly mentioned. This policy explains what information Kuyo uses and how it is handled.

## Information we use

Kuyo uses only the information needed to provide its features:

- Discord server, channel, and user IDs
- Server settings, voice preferences, and custom pronunciation entries
- Messages posted in the text channel selected by a server administrator
- Non-empty messages that explicitly mention Kuyo, for the character reply feature
- Display names and the names of mentioned users, roles, or channels when needed to read a message naturally

Kuyo does not collect passwords, payment information, contacts, or direct messages. Outside the selected TTS channel, it processes a message only when that message explicitly mentions Kuyo and contains other text.

## How information is used

Message text is prepared for speech and sent to Microsoft Edge Read Aloud by default. If the service operator enables Google Chirp 3 HD, text is sent to Google Cloud Text-to-Speech and falls back to Microsoft Edge Read Aloud when Google fails before returning audio or does not support the detected language. The generated audio is played in the connected Discord voice channel.

When a non-empty message explicitly mentions Kuyo, the text is reduced to remove Discord identifiers and URLs, limited in length, and sent to the OpenAI Responses API. GPT-5.6 Luna writes Kuyo's short reply in the language of the message. Application code then checks that reply against a fixed grammar — a length limit, letters and simple punctuation only, and no digits, links, mentions, or markup — and replaces it with a curated character line if it does not fit. Each request contains only the current message and Kuyo's own previous line; no conversation history is sent or kept. API response storage is disabled for these requests. Messages without an explicit Kuyo mention, and mentions with no other text, are not sent to OpenAI.

Kuyo does not sell personal information, show advertising, create user profiles, or use message content for tracking.

## Storage and retention

Kuyo does not save message text, generated audio, or conversation history. Kuyo's own most recent line per user is held in memory only, to avoid repeating herself, and is lost when the bot restarts.

Server settings and pronunciation entries are kept while the bot remains in the server. They are deleted when the bot is removed. Voice preferences are shared across servers that use Kuyo and remain until the user deletes them or the service is discontinued.

Limited service logs may contain server IDs, timing information, and error messages. Message text is not written to these logs. Logs are automatically rotated and used only to keep the service reliable.

## Service providers

Kuyo relies on the following providers:

- [Discord](https://discord.com/privacy) for messages, commands, and voice connections
- [Microsoft](https://privacy.microsoft.com/privacystatement) for primary speech generation
- [Google Cloud](https://cloud.google.com/terms/cloud-privacy-notice) for optional speech generation when enabled by the service operator
- [OpenAI](https://openai.com/policies/privacy-policy/) for writing Kuyo's short character reply after an explicit mention

These providers may process information in countries outside your own and apply their own privacy terms.

## Your choices and rights

Use `/privacy show` to see the voice settings linked to your Discord account. Use `/privacy delete` to delete them.

Server administrators can view or remove custom pronunciation entries with `/dictionary list` and `/dictionary remove`. Removing Kuyo from a server deletes that server's settings and pronunciation entries.

For any other privacy request, contact the administrator who added Kuyo to your Discord server. Do not post personal information in a public issue or channel.

## Age requirements

Kuyo is intended for people who are old enough to use Discord in their country. It is not directed to children below that age.

## Changes

This policy may be updated when Kuyo changes. The effective date at the top will be revised when material changes are made.
