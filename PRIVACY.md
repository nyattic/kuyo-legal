# Kuyo Privacy Policy

Effective: August 5, 2026

Kuyo is a Discord bot that reads selected text messages aloud in a voice channel. This policy explains what information Kuyo uses and how it is handled.

## Information we use

Kuyo uses only the information needed to provide its features:

- Discord server, channel, and user IDs
- Server settings, voice preferences, and custom pronunciation entries
- Messages posted in the text channel selected by a server administrator
- Display names and the names of mentioned users, roles, or channels when needed to read a message naturally

Kuyo does not collect passwords, payment information, contacts, direct messages, or activity outside the selected text channel.

## How information is used

Message text is prepared for speech and sent to Google Cloud Text-to-Speech by default. If Google fails before returning audio or does not support the detected language, the text is sent to Microsoft Edge Read Aloud as a fallback. The generated audio is played in the connected Discord voice channel.

Kuyo does not sell personal information, show advertising, create user profiles, or use message content for tracking.

## Storage and retention

Kuyo does not save message text or generated audio.

Server settings and pronunciation entries are kept while the bot remains in the server. They are deleted when the bot is removed. Voice preferences are shared across servers that use Kuyo and remain until the user deletes them or the service is discontinued.

Limited service logs may contain server IDs, timing information, and error messages. Message text is not written to these logs. Logs are automatically rotated and used only to keep the service reliable.

## Service providers

Kuyo relies on the following providers:

- [Discord](https://discord.com/privacy) for messages, commands, and voice connections
- [Google Cloud](https://cloud.google.com/terms/cloud-privacy-notice) for primary speech generation
- [Microsoft](https://privacy.microsoft.com/privacystatement) for fallback speech generation

These providers may process information in countries outside your own and apply their own privacy terms.

## Your choices and rights

Use `/privacy show` to see the voice settings linked to your Discord account. Use `/privacy delete` to delete them.

Server administrators can view or remove custom pronunciation entries with `/dictionary list` and `/dictionary remove`. Removing Kuyo from a server deletes that server's settings and pronunciation entries.

For any other privacy request, contact the administrator who added Kuyo to your Discord server. Do not post personal information in a public issue or channel.

## Age requirements

Kuyo is intended for people who are old enough to use Discord in their country. It is not directed to children below that age.

## Changes

This policy may be updated when Kuyo changes. The effective date at the top will be revised when material changes are made.
