# Kumikuyo Privacy Policy

Effective: August 4, 2026

Kumikuyo is a Discord bot that reads selected text messages aloud in a voice channel. This policy explains what information Kumikuyo uses and how it is handled.

## Information we use

Kumikuyo uses only the information needed to provide its features:

- Discord server, channel, and user IDs
- Server settings, voice preferences, and custom pronunciation entries
- Messages posted in the text channel selected by a server administrator
- Display names and the names of mentioned users, roles, or channels when needed to read a message naturally

Kumikuyo does not collect passwords, payment information, contacts, direct messages, or activity outside the selected text channel.

## How information is used

Message text is prepared for speech and sent to Google Cloud Text-to-Speech. If Google is unavailable, or if the selected language is not supported there, the text may be sent to Microsoft Edge Read Aloud instead. The generated audio is played in the connected Discord voice channel.

Kumikuyo does not sell personal information, show advertising, create user profiles, or use message content for tracking.

## Storage and retention

Kumikuyo does not save message text or generated audio.

Server settings and pronunciation entries are kept while the bot remains in the server. They are deleted when the bot is removed. Voice preferences are shared across servers that use Kumikuyo and remain until the user deletes them or the service is discontinued.

Limited service logs may contain server IDs, timing information, and error messages. Message text is not written to these logs. Logs are automatically rotated and used only to keep the service reliable.

## Service providers

Kumikuyo relies on the following providers:

- [Discord](https://discord.com/privacy) for messages, commands, and voice connections
- [Google Cloud](https://cloud.google.com/terms/cloud-privacy-notice) for primary speech generation
- [Microsoft](https://privacy.microsoft.com/privacystatement) for backup speech generation

These providers may process information in countries outside your own and apply their own privacy terms.

## Your choices and rights

Use `/privacy show` to see the voice settings linked to your Discord account. Use `/privacy delete` to delete them.

Server administrators can view or remove custom pronunciation entries with `/dictionary list` and `/dictionary remove`. Removing Kumikuyo from a server deletes that server's settings and pronunciation entries.

For any other privacy request, contact the administrator who added Kumikuyo to your Discord server. Do not post personal information in a public issue or channel.

## Age requirements

Kumikuyo is intended for people who are old enough to use Discord in their country. It is not directed to children below that age.

## Changes

This policy may be updated when Kumikuyo changes. The effective date at the top will be revised when material changes are made.
