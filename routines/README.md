# Cloud Routines

These are the **production** prompts. Each file is pasted verbatim into a Claude
Code cloud routine. Each routine is an ephemeral container: clone → run → destroy.
**If it's not committed and pushed to `main`, it didn't happen.**

## One-time prerequisites

1. **Install the Claude GitHub App** on this repo (clone + push permission).
   Or run `/web-setup` in Claude Code to sync your `gh` token.
2. **Enable "Allow unrestricted branch pushes"** on each routine's environment.
   Without this, `git push origin main` silently fails with a proxy error — the
   #1 cause of broken first-time setups.
3. **Set environment variables on the routine** (NOT a committed `.env`):
   - `ALPACA_API_KEY` (required)
   - `ALPACA_SECRET_KEY` (required)
   - `ALPACA_ENDPOINT` (optional; defaults to live URL)
   - `ALPACA_DATA_ENDPOINT` (optional; defaults to data URL)
   - `PERPLEXITY_API_KEY` (required for research)
   - `PERPLEXITY_MODEL` (optional; defaults to `sonar`)
   - `CLICKUP_API_KEY` (required for notifications)
   - `CLICKUP_WORKSPACE_ID` (required; numeric)
   - `CLICKUP_CHANNEL_ID` (required; format `4-XXXXXXX-X`)

## The five schedules (America/Chicago)

| Routine        | Cron            |
|----------------|-----------------|
| pre-market     | `0 6 * * 1-5`   |
| market-open    | `30 8 * * 1-5`  |
| midday         | `0 12 * * 1-5`  |
| daily-summary  | `0 15 * * 1-5`  |
| weekly-review  | `0 16 * * 5`    |

## Creating a routine

1. Routines → New Routine → name it.
2. Select this repo + branch `main`.
3. Add all env vars above.
4. Toggle on **Allow unrestricted branch pushes**.
5. Set the cron + timezone.
6. Paste the matching `routines/*.md` prompt **verbatim** (do not paraphrase —
   the env-var check and the commit-and-push step are load-bearing).
7. Save, then **Run now** to test. Don't wait until tomorrow to find it's broken.
