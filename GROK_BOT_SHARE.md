# Publish the official Grok Bot share link

xAI does not expose an API to publish a Bot from this repo. You publish from the Grok Bot app. This file is the exact sanitized checklist.

## Before you tap Share

Delete from the bot (instructions, memories, files, routines):

- SSN, Medicaid ID, SSA claim numbers
- Bank, wallet seed, API keys
- Home address, kids names, medical detail
- Exact SSI dollar amounts
- Internal LVL / DogeForge treasury keys
- Any conversation that contains the above

Keep only the job instructions from `agents/grant-packet-assembler.md`.

## Publish

1. Open the Grant Packet Assembler bot.
2. Share a Bot → scope **Public** (not team-only).
3. Inspect the preview page. Confirm no personal facts leaked.
4. Copy the `https://x.ai/bot/...` URL.
5. Paste that URL into `listings/SHARE_URL.txt` and commit it.
6. Post the X draft in `listings/x-post.md` with that URL filled in.
7. Open a PR on grokbot.dev using `listings/grokbot-dev-plugin.md`.

## After publish

Treat the share link as world-readable. If you later add a memory with private facts, create a **new** bot for public share. Do not re-share the private working copy.
