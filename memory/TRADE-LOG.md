# Trade Log

## Day 0 — EOD Snapshot (pre-launch baseline)
**Portfolio:** $10,000.00 | **Cash:** $10,000.00 (100%) | **Day P&L:** $0 | **Phase P&L:** $0

No positions yet. Bot launches tomorrow.

## Jun 10 — EOD Snapshot (Day 1, Wednesday)
**Portfolio:** $100,000.00 | **Cash:** $100,000.00 (100%) | **Day P&L:** $0 (0%) | **Phase P&L:** $0 (0%)

No positions. No trades.

Notes: Account funded and active as of today, but Alpaca equity is $100,000.00 vs the $10,000 baseline recorded on Day 0 / in PROJECT-CONTEXT.md and TRADING-STRATEGY.md — a 10x mismatch (likely default paper account funding). Flagged to user via ClickUp; treating $100,000.00 as the working baseline for Phase P&L going forward until confirmed/corrected. No positions, no orders, no trades today (account just came online). PDT count: 0.

## Jun 11 — Trade (Day 2, Thursday)
**BUY XLE** — 300 sh @ $58.57 entry | cost $17,571 (17.6% equity)
- Stop: 10% trailing GTC, initial floor $52.76 (hwm $58.62) [order 3e8a4aca]
- Thesis: Post-PPI entry. May PPI benign (+0.1% MoM vs +0.2% exp, 3.0% YoY vs 3.1%) cleared binary risk. Energy YTD leader + oil firmed (~$92 WTI). Defensive rotation confirming intraday — XLE +0.6%, XLP +1.0% green while SPY -0.7%, XLI -1.2% red. XLE cleared 58.5 entry-on-strength trigger.
- Target: +16% (~$67.9). R:R ~1.6:1 (10% trail). 
- Trades this week: 1/3. Positions: 1/6. Deployed: ~17.6%.

## Jun 11 — EOD Snapshot (Day 2, Thursday)
**Portfolio:** $99,562.00 | **Cash:** $82,429.00 (82.8%) | **Day P&L:** -$438.00 (-0.44%) | **Phase P&L:** -$438.00 (-0.44%)

| Ticker | Shares | Entry | Close | Day Chg | Unrealized P&L | Stop |
|--------|--------|-------|-------|---------|----------------|------|
| XLE | 300 | $58.57 | $57.11 | -1.96% | -$438 (-2.49%) | $52.97 trail 10% GTC (hwm $58.86) |

Notes: Day 2. Opened first position — 300 sh XLE @ $58.57 on the post-PPI defensive-rotation thesis, 10% trailing stop live as GTC [3e8a4aca]. XLE faded into the close (-1.96% on the day), leaving the position at -2.49% unrealized / -$438, which is the entirety of today's portfolio drawdown. Still well inside risk limits: -2.49% vs -7% manual-cut line and far above the $52.97 trailing stop. Deployed only ~17% (1/6 positions, 1/3 weekly trades used) — below the 75-85% target, so capital remains for adds as thesis develops. No stops triggered, no other trades. PDT count: 0.

## Jun 12 — EOD Snapshot (Day 3, Friday)
**Portfolio:** $99,678.99 | **Cash:** $82,428.99 (82.7%) | **Day P&L:** +$116.99 (+0.12%) | **Phase P&L:** -$321.01 (-0.32%)

| Ticker | Shares | Entry | Close | Day Chg | Unrealized P&L | Stop |
|--------|--------|-------|-------|---------|----------------|------|
| XLE | 300 | $58.57 | $57.50 | +0.67% | -$321 (-1.83%) | $52.97 trail 10% GTC (hwm $58.86) |

Notes: Day 3. No trades today — held the single XLE position. XLE recovered modestly (+0.67%), trimming unrealized loss to -$321 / -1.83% from yesterday's -2.49%, and lifting the portfolio +$116.99 (+0.12%) on the day. Phase P&L now -0.32%, essentially the XLE unrealized mark. Position well inside limits: -1.83% vs -7% cut line, far above $52.97 trailing stop (10% GTC live [3e8a4aca], hwm $58.86). Deployed ~17.3% (1/6 positions), below the 75-85% target — dry powder remains. Weekly trade count 1/3, week closes Friday. PDT count: 0. Next week: monitor energy/oil thesis on XLE; scout adds to lift deployment toward target if pre-market research confirms momentum.

## Jun 15 — Market-Open (Day 4, Monday) — XLE EXIT ATTEMPT FAILED (broker)
**Plan:** Exit XLE per today's RESEARCH-LOG — thesis broken on both legs (WTI ~$80, -20% on Iran de-escalation; rotation reversed tech-ward; XLE below 50-DMA). Position -5.8% unrealized. Do not defend a dead thesis into FOMC 6/17.
**Action attempted:** Canceled 10% trailing stop [3e8a4aca], submitted market sell 300 XLE to close.
**Outcome: NOT FILLED.** Market sell sat in `new` >2 min with zero fill during regular hours (liquid ETF) — Alpaca paper fill engine not executing. Resubmitted [35b35373] — same, no fill. Canceled both.
**Protection restored:** Re-placed protective stop — fixed stop $52.97 GTC [ee73ba2c] at the prior trail level (a fresh 10% trailing stop reset its hwm to $55.12 → floor $49.61, which would move the stop DOWN, so used fixed $52.97 to honor never-move-down). Position protected, NOT naked.
**State:** XLE 300 sh @ $58.57, cur ~$55.14, -5.8%. 1/6 positions, 0/3 weekly trades used. daytrade_count 0.
**Next:** Retry full exit at midday run once fills are processing. Alerted user via ClickUp.

## Jun 15 — Midday EXIT FILLED (Day 4, Monday) — XLE CLOSED
**SELL XLE** — 300 sh @ $55.90 exit (market sell-to-close [2c4fbc4d], filled 17:05 UTC) | proceeds $16,770
- Entry $58.57 → exit $55.90 = **realized -$801.00 (-4.56%)**
- Reason: thesis broken (not a -7% cut). Morning RESEARCH-LOG killed the XLE thesis on both legs — WTI ~$80 (-20% on Iran de-escalation) and rotation reversed tech-ward, XLE below 50-DMA. Do not defend a dead thesis into FOMC 6/17.
- Execution: morning market-sell attempts sat unfilled (paper engine). Midday retry — canceled protective stop [ee73ba2c] (204), submitted market sell to close, FILLED in <1s @ $55.90.
- State after: 0/6 positions, 100% cash. Account $99,198.99. Weekly trades 0/3 (exit doesn't count as new trade). daytrade_count 0 (entry 6/11, exit 6/15 — not a day trade). No open orders, no naked exposure.
- Next: redeploy per pre-market research; energy thesis dead, stay patient into FOMC 6/17.

## Jun 15 — EOD Snapshot (Day 4, Monday)
**Portfolio:** $99,198.99 | **Cash:** $99,198.99 (100%) | **Day P&L:** -$480.00 (-0.48%) | **Phase P&L:** -$801.01 (-0.80%)

No open positions. 100% cash.

Notes: Day 4. Closed the lone XLE position today at midday — sold 300 sh @ $55.90 for a realized -$801.00 (-4.56%) after the morning RESEARCH-LOG killed the thesis on both legs (WTI ~$80, -20% on Iran de-escalation; rotation reversed tech-ward, XLE below 50-DMA). Not a -7% stop-out — a disciplined thesis-broken exit ahead of FOMC 6/17. Morning market-sell attempts sat unfilled in the paper engine and a protective fixed stop $52.97 GTC was held in the interim; midday retry filled in <1s. Day P&L -$480 / -0.48%; Phase P&L now -$801 / -0.80%, essentially the realized XLE loss since the book is flat. Account $99,198.99, 100% cash, 0/6 positions, no open orders, no naked exposure. Weekly new-trade count 0/3 (exit doesn't count). daytrade_count 0 (entry 6/11, exit 6/15 — not a day trade). PDT false. Next: redeploy per pre-market research; energy thesis dead, stay patient into FOMC 6/17.

## Jun 16 — EOD Snapshot (Day 5, Tuesday)
**Portfolio:** $99,198.93 | **Cash:** $99,198.93 (100%) | **Day P&L:** -$0.06 (-0.00%) | **Phase P&L:** -$801.07 (-0.80%)

No open positions. 100% cash.

Notes: Day 5. No trades, no positions, no open orders — held 100% cash through the session, so the book was unchanged and Day P&L is flat (-$0.06, rounding). Phase P&L holds at -$801.07 / -0.80%, still just the realized XLE loss from Monday. Deliberately sidelined ahead of the FOMC decision tomorrow (6/17) — no sense opening fresh risk into a binary macro event with the prior (energy) thesis dead. Dry powder fully intact for post-FOMC redeployment if pre-market research confirms a new setup. Weekly new-trade count 0/3, daytrade_count 0, PDT false. Next: pre-market research 6/17, then react to FOMC; stay patient, deploy toward the 75-85% target only on a confirmed thesis.

## Jun 17 — EOD Snapshot (Day 6, Wednesday)
**Portfolio:** $99,198.93 | **Cash:** $99,198.93 (100%) | **Day P&L:** $0.00 (0.00%) | **Phase P&L:** -$801.07 (-0.80%)

No open positions. 100% cash.

Notes: Day 6, FOMC decision day. No trades, no positions, no open orders — held 100% cash through the session, so the book was unchanged and Day P&L is flat ($0.00). Phase P&L holds at -$801.07 / -0.80%, still just the realized XLE loss from Monday. Stayed deliberately sidelined through the FOMC decision rather than open fresh risk into the binary macro event with the prior (energy) thesis dead and no confirmed replacement setup. Dry powder fully intact for post-FOMC redeployment if pre-market research confirms a new thesis. Weekly new-trade count 0/3, daytrade_count 0, PDT false. Next: pre-market research 6/18 to digest the FOMC outcome/SEP/dot-plot and scout a confirmed setup; deploy toward the 75-85% target only on conviction — patience > activity.

## Jun 18 — EOD Snapshot (Day 7, Thursday)
**Portfolio:** $99,198.93 | **Cash:** $99,198.93 (100%) | **Day P&L:** $0.00 (0.00%) | **Phase P&L:** -$801.07 (-0.80%)

No open positions. 100% cash.

Notes: Day 7, first session post-FOMC. No trades, no positions, no open orders — held 100% cash through the session, so the book was unchanged and Day P&L is flat ($0.00). Phase P&L holds at -$801.07 / -0.80%, still just the realized XLE loss from Monday. Did not redeploy: with the prior (energy) thesis dead and no confirmed replacement setup off the FOMC digest, opening fresh risk would violate patience > activity. Dry powder fully intact (0/6 positions, 0% deployed vs 75-85% target) for a conviction entry once pre-market research confirms a thesis. Weekly new-trade count 0/3, daytrade_count 0, PDT false. Next: pre-market research 6/19 to scout a confirmed post-FOMC setup; deploy toward target only on conviction, ahead of Friday's weekly review.

## Jun 19 — EOD Snapshot (Day 8, Friday)
**Portfolio:** $99,198.93 | **Cash:** $99,198.93 (100%) | **Day P&L:** $0.00 (0.00%) | **Phase P&L:** -$801.07 (-0.80%)

No open positions. 100% cash.

Notes: Day 8, second session post-FOMC. No trades, no positions, no open orders — held 100% cash through the session, so the book was unchanged and Day P&L is flat ($0.00). Phase P&L holds at -$801.07 / -0.80%, still just the realized XLE loss from Monday. Did not redeploy: with the prior (energy) thesis dead and no confirmed replacement setup, opening fresh risk would violate patience > activity. Dry powder fully intact (0/6 positions, 0% deployed vs 75-85% target) for a conviction entry once pre-market research confirms a thesis. Weekly new-trade count 0/3, daytrade_count 0, PDT false. Note: this is the fourth straight flat/cash session (Tue-Fri) — extended idleness vs the 75-85% deployment mandate; weekly review due this afternoon should address the lack of a confirmed setup and whether the screening process is too restrictive. Next: weekly review, then pre-market research Monday to scout a confirmed setup; deploy toward target only on conviction.

## Jun 22 — EOD Snapshot (Day 9, Monday)
**Portfolio:** $99,198.93 | **Cash:** $99,198.93 (100%) | **Day P&L:** $0.00 (0.00%) | **Phase P&L:** -$801.07 (-0.80%)

No open positions. 100% cash.

Notes: Day 9, start of a new week. No trades, no positions, no open orders — held 100% cash through the session, so the book was unchanged and Day P&L is flat ($0.00). Phase P&L holds at -$801.07 / -0.80%, still just the realized XLE loss from Jun 15. Did not redeploy: no confirmed replacement setup, so opening fresh risk would violate patience > activity. Dry powder fully intact (0/6 positions, 0% deployed vs 75-85% target). Weekly new-trade count 0/3, daytrade_count 0, PDT false. CONCERN: this is now the FIFTH straight flat/cash session (Tue 6/16 → Mon 6/22) — the book has been fully idle for a full trading week against the 75-85% deployment mandate. The screening process is producing no actionable theses; pre-market research needs to either surface a conviction setup or the strategy's screen criteria should be revisited. Capital is earning nothing while sidelined. Next: pre-market research Tuesday 6/23 must produce a confirmed setup to begin redeploying toward target — idleness is now the primary risk, not a market event.
