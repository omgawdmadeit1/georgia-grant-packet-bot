# Listing PRs

## grokbot.dev (file is on the fork)

Open this compare and create the PR:

https://github.com/ZeroPointRepo/GrokBotDev/compare/main...omgawdmadeit1:add-georgia-grant-packet?expand=1

## Official Grok Build plugin marketplace

Fork: https://github.com/omgawdmadeit1/plugin-marketplace/tree/add-georgia-grant-packet

Catalog entry to add is in `listings/marketplace-catalog-entry.json`.
Then run in a clone of the fork:

```bash
python3 scripts/generate-plugin-index.py
python3 scripts/validate-catalog.py
python3 scripts/generate-plugin-index.py --check
```

Compare:

https://github.com/xai-org/plugin-marketplace/compare/main...omgawdmadeit1:add-georgia-grant-packet?expand=1

The GitHub connector in this session cannot open PRs on those upstream repos (403).
