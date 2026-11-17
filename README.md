# Binance

Use `binance-cli` for Binance Spot, Futures (USD-S), and Convert — from an agent skill (v2.1.0, by Binance).

## What it is

A skill that drives the official Binance CLI: spot trading, USDⓈ-M and COIN-M futures, options, convert, C2C, copy trading, algo trading, crypto loans, dual investment, and market-data streams.

## What's inside

- `SKILL.md` — the skill definition and command map
- `references/` — one reference file per command group (`auth.md`, `futures-usds.md`, `convert.md`, `algo.md`, …)

## Setup

Install the CLI:

```sh
curl --proto '=https' --tlsv1.2 -LsSf \
  https://github.com/binance/binance-cli/releases/latest/download/binance-cli-installer.sh \
  | sh
```

Verify:

```sh
binance-cli --version
```

> **Prerequisite:** read [`references/auth.md`](references/auth.md) for auth, global flags, and security rules before running any command.

## Command groups

| Group | Covers |
|---|---|
| Spot & Convert | `convert`, `fiat`, `c2c` |
| Futures | `futures-usds`, `futures-coin`, options, portfolio margin |
| Trading | `algo`, `copy-trading`, `dual-investment`, `crypto-loan` |
| Data | market streams, CMS streams, Alpha |

## Security

API keys are credentials: keep them in the agent's secure store, never paste them in chat, logs, or files. Use IP restrictions and withdrawal-disabled keys where possible.

## Risk warning

Trading on Binance — especially leveraged futures — can lose money fast. This skill is a tool, not financial advice.

## License

MIT — see [LICENSE](LICENSE).
