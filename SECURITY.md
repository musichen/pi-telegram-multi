# Security Policy

## Reporting a vulnerability

Open a GitHub issue in this repository for non-sensitive reports. For a sensitive vulnerability, contact the maintainer privately first through the GitHub profile at https://github.com/musichen instead of posting details publicly.

Please include the extension version or commit, your pi version, and steps to reproduce. Redact bot tokens and Telegram user IDs from logs and screenshots.

## Notes for users

- Bot config files under `~/.pi/agent/` (for example `telegram-<bot-username>.json`) contain `botToken` secrets. Keep them private, do not commit them, and rotate a token with @BotFather if one leaks.
- Extensions run with your full system permissions. Only add numeric Telegram user IDs you trust to `allowedUserIds`, since an allowlisted account can drive the pi session through Telegram.
- Connect each bot to only one pi session at a time, and disconnect bots you no longer use with `/telegram-disconnect`.
