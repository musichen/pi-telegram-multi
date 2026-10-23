# Contributing to pi-telegram-multi

## Setup

Install pi, then load the extension from your checkout for testing:

```bash
pi -e ./index.ts
```

Or install your fork with `pi install git:github.com/<you>/pi-telegram-multi` as described in the README.

## Test manually

1. Create a test bot with @BotFather.
2. Run `/telegram-setup` and `/telegram-connect`, then send `/start` from Telegram.
3. Check `/telegram-status` shows the right bot, config, and allowed users.
4. For allowlist changes, remember only numeric Telegram user IDs work, and reconnect after editing the config.

There is no automated test script yet, so describe your manual test in the pull request.

## Pull requests

Create a branch from `main`, keep the change focused on `index.ts` or the README, and describe the bot setup you tested with (redact bot tokens).
