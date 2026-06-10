# Trading Bot

An autonomous, cloud-scheduled swing-trading agent built on Claude Code. Claude
*is* the bot — there is no separate Python process. Five cron-scheduled cloud
routines fire each weekday; each one clones this repo, reads memory, pulls live
Alpaca state, decides, trades, writes memory, and pushes back to `main`.

## Architecture

- **Stateless runs** — each firing is an independent, ephemeral container.
- **Git as memory** — all state lives in `memory/*.md`, committed to `main`.
- **Hard rules as gates** — strategy discipline is enforced before every order.

## Layout

```
CLAUDE.md            Agent rulebook (auto-loaded every session)
env.template         Template for local .env (cloud uses routine env vars)
.claude/commands/    Ad-hoc slash commands for local use
routines/            Cloud routine prompts (the production path)
scripts/             API wrappers — the only way to touch the outside world
memory/              Agent's persistent state (committed to main)
```

## Local quickstart

1. `cp env.template .env` and fill in your credentials.
2. `chmod +x scripts/*.sh`
3. Open this repo in Claude Code and run `/portfolio` for a read-only snapshot.

> Wrapper scripts are bash + `curl` + `python`. On Windows, run them via Git Bash
> / WSL. Cloud routines run in Linux containers, so bash is always available there.

## Cloud deployment

See `routines/README.md` and the setup guide. Key prerequisites:

1. Install the Claude GitHub App on this repo (clone + push permission).
2. Enable **"Allow unrestricted branch pushes"** on each routine's environment.
3. Set all credentials as **routine environment variables** — never a committed `.env`.

## The five daily routines (America/Chicago)

| Routine        | Cron            | When                         |
|----------------|-----------------|------------------------------|
| pre-market     | `0 6 * * 1-5`   | 6:00 AM weekdays             |
| market-open    | `30 8 * * 1-5`  | 8:30 AM weekdays (the bell)  |
| midday         | `0 12 * * 1-5`  | noon weekdays                |
| daily-summary  | `0 15 * * 1-5`  | 3:00 PM weekdays (close)     |
| weekly-review  | `0 16 * * 5`    | 4:00 PM Fridays only         |

## Safety

This bot can place **real orders** against a live brokerage account. Start on
Alpaca **paper** trading, monitor the first week closely, and read every commit
the agent makes. Never commit a real `.env`.
