# Georgia Grant Packet Bot

A Grok Bot teammate and Grok Build plugin that assembles **SSI-safe** grant and self-employment packets for Georgia programs:

- OneGeorgia / rural economic development
- GVRA self-employment supports
- SBDC counseling packages
- DOBE certification pathway
- PASS (Plan to Achieve Self-Support) drafting support

It researches official sources, drafts narrative + budget + attachment checklists, and **stops before any submit, email, portal upload, or payment**.

## What this is not

- Not a lawyer, SSA claims representative, or guaranteed-award service.
- Not a place to store SSN, bank numbers, medical records, or benefit amounts.
- Not an auto-submitter. Human confirms every outbound action.

## Install in Grok Build

After this plugin is accepted into the official catalog:

```bash
grok plugin marketplace list
grok plugin install georgia-grant-packet --trust
```

Until then, clone this repo and add it as a local marketplace source.

## Install as a Grok Bot teammate

1. Open Grok Bot → **+** → **Create New Bot**.
2. Name it `Grant Packet Assembler`.
3. Paste the contents of `agents/grant-packet-assembler.md` into Instructions.
4. Attach the skill at `skills/georgia-grant-packet/SKILL.md` if your client supports skill files.
5. Share → **Public** only after you have removed any personal facts you typed during testing.
6. Copy the `x.ai/bot/...` share link.

Full share checklist: `GROK_BOT_SHARE.md`.

## Network endpoints this plugin uses

Read-only official research. No credentials required.

- `https://www.onegeorgia.org`
- `https://gvs.georgia.gov` and GVRA public pages
- `https://www.georgiasbdc.org`
- `https://www.ssa.gov` (PASS / SSI public pages only)
- Georgia DBHDD and White County / rural development public pages as needed

The bot must cite the live URL it fetched. It must not invent deadlines or award amounts.

## Security

- No postinstall scripts.
- No shell hooks.
- No secret collection.
- Writes stay in the working folder the user names.
- Submit / send / pay require an explicit human sentence that includes the word **send**, **submit**, or **pay** for that specific artifact.

## License

MIT. See `LICENSE`.

Homepage: https://lvlltd.com  
Repo: https://github.com/omgawdmadeit1/georgia-grant-packet-bot
