# Weekly Review

Friday reviews appended here.

Template for each entry:

## Week ending YYYY-MM-DD

### Stats
| Metric | Value |
|--------|-------|
| Starting portfolio | $X |
| Ending portfolio | $X |
| Week return | ±$X (±X%) |
| S&P 500 week | ±X% |
| Bot vs S&P | ±X% |
| Trades | N (W:X / L:Y / open:Z) |
| Win rate | X% |
| Best trade | SYM +X% |
| Worst trade | SYM -X% |
| Profit factor | X.XX |

### Closed Trades
| Ticker | Entry | Exit | P&L | Notes |

### Open Positions at Week End
| Ticker | Entry | Close | Unrealized | Stop |

### What Worked
- ...

### What Didn't Work
- ...

### Key Lessons
- ...

### Adjustments for Next Week
- ...

### Overall Grade: X

## Week ending 2026-06-12

### Stats
| Metric | Value |
|--------|-------|
| Starting portfolio | $100,000.00 (Wed 6/10 launch, working baseline) |
| Ending portfolio | $99,693.75 |
| Week return | -$306.25 (-0.31%) |
| S&P 500 week | -0.1% |
| Bot vs S&P | -0.21% |
| Trades | 1 (W:0 / L:0 / open:1) |
| Win rate | N/A (no closed trades) |
| Best trade | XLE -1.74% (open) |
| Worst trade | XLE -1.74% (open) |
| Profit factor | N/A (no closed trades) |

### Closed Trades
| Ticker | Entry | Exit | P&L | Notes |
| — | — | — | — | None closed this week |

### Open Positions at Week End
| Ticker | Entry | Close | Unrealized | Stop |
| XLE | $58.57 | $57.55 | -$306 (-1.74%) | $52.97 trail 10% GTC (hwm $58.86) [3e8a4aca] |

### What Worked
- Discipline into binary events — sat out CPI (6/10) and PPI (6/11) prints rather than deploying into them. CPI came in hot; not being positioned avoided the Wed selloff.
- Entered XLE on a defined post-PPI strength trigger (>58.5) with a written thesis, not a reflex.
- Risk controls clean: 10% trailing GTC stop live from entry, position never near the -7% cut line.
- Stayed well inside all caps — 1/6 positions, 1/3 weekly trades, no PDT flags.

### What Didn't Work
- XLE thesis decayed fast: oil dropped ~4% on 6/12 and rotation flipped tech-ward (NQ +3.26% Thu), undercutting both legs of the defensive-energy trade. Position underwater all week.
- Under-deployed at ~17% vs the 75-85% target for the whole week — capital sat idle, no chance to beat the index.
- Slightly trailed the S&P (-0.31% vs -0.1%) — the lone position was the entire drag.

### Key Lessons
- A single-position, ~17% book can only match cash, not beat the benchmark. Need breadth to compete.
- Energy/defensive leadership is fragile when oil rolls and tech rotation resumes — confirm the oil tape before adding to XLE.
- Sitting out event risk was correct and repeatable; keep it.

### Adjustments for Next Week
- FOMC 6/16-17 is the week's binary — do NOT deploy fresh capital into the decision; build after.
- Post-FOMC, work deployment toward 75-85% with 2-4 names if momentum confirms; don't force trades into the event.
- Re-engage XLE only on a reclaim of $58 with oil stabilizing; otherwise honor $52.97 trail / $54.47 manual line.
- Diversify beyond energy — watch the tech/AI leadership flip for a pullback entry.

### Overall Grade: C
- Capital preserved and risk-managed (good), but under-deployed and modestly behind the S&P with no closed wins. Average week — disciplined, not productive.

## Week ending 2026-06-19

### Stats
| Metric | Value |
|--------|-------|
| Starting portfolio | $99,678.99 (Mon 6/15 AM ≈ Fri 6/12 close) |
| Ending portfolio | $99,198.93 |
| Week return | -$480.06 (-0.48%) |
| S&P 500 week | +0.93% (Mon–Thu; Fri 6/19 closed, Juneteenth) |
| Bot vs S&P | -1.41% |
| Trades | 1 (W:0 / L:1 / open:0) |
| Win rate | 0% (1 closed) |
| Best trade | XLE -4.56% (only trade) |
| Worst trade | XLE -4.56% |
| Profit factor | 0.00 (no winners) |

### Closed Trades
| Ticker | Entry | Exit | P&L | Notes |
| XLE | $58.57 | $55.90 | -$801 (-4.56%) | Thesis-broken exit 6/15 (not -7% stop). WTI -20% on Iran de-escalation; rotation flipped tech-ward; XLE below 50-DMA. Closed pre-FOMC. |

### Open Positions at Week End
| Ticker | Entry | Close | Unrealized | Stop |
| — | — | — | — | None — 100% cash since 6/15 |

### What Worked
- Cut the dead XLE thesis decisively at -4.56% rather than riding it to the -7% line or into FOMC — disciplined exit on broken-thesis logic, both legs (oil, rotation) objectively gone.
- Sat out the FOMC 6/17 binary in cash — the hawkish hold (median dots 3.8%, ~half see a hike, CPI 4.2%) gapped SPX -1.21% Wed; not being positioned avoided that drawdown.
- Risk controls clean all week: re-armed a fixed protective stop when the paper fill engine stalled on the morning exit (honored never-move-down), never naked, never near a real loss line.
- Zero rule violations: 0/3 weekly trades, 0/6 positions, no PDT flags, daytrade_count 0.

### What Didn't Work
- Chronic under-deployment, now a 2-week pattern: 100% cash Tue–Fri while the mandate is 75-85% deployed. Cash cannot beat an up market — S&P rose +0.93% and we booked -0.48%, a -1.41% miss.
- Never pulled the trigger on the prepared XLI lead. The FOMC sideline reason was resolved by Thu, yet the entry precondition ("tape green, holds opening range") kept deferring — defensible each day, but the cumulative effect is full non-participation.
- The one realized trade was a loss; phase record is 0-for-1 closed, -$801 / -0.80% phase, entirely the XLE round trip.
- "Patience > activity" is doing real work as a discipline anchor but is sliding toward paralysis — every session this week resolved to "wait for Monday."

### Key Lessons
- Discipline that never deploys is just cash drag. Two weeks in, the bot has never exceeded ~17% deployed and has trailed the S&P both weeks — the binding constraint is not risk, it's failure to enter.
- A precondition that can defer indefinitely ("tape green at the open") needs a hard backstop: a date/level by which we either take the prepared trade or formally pass, so we stop rolling the same idea forward day after day.
- Sitting out a true binary (FOMC) was correct; sitting out the two clean post-event sessions was the actual cost.

### Adjustments for Next Week
- Monday 6/22: take the prepared XLI entry on confirmed opening strength (tape green / holds opening range), ~20% sizing, stop -8%, target +16%, 10% trailing GTC from fill. If Monday's open is red, pass on XLI but actively screen a second non-energy leader (Materials/Staples) rather than defaulting to all-cash.
- Set a deployment floor as an operating discipline (not yet a hard rule): be at ≥40% deployed by Wed 6/24 unless a fresh binary event or a broken tape justifies cash — force the question instead of passively waiting.
- Build breadth toward 2-4 names and the 75-85% target as setups confirm; energy stays OFF (broken thesis, WTI ~$77), tech only on a clean re-acceleration vs the hawkish-dots headwind.
- No strategy hard-rule change this week — the framework is sound; the gap is execution. Re-evaluate the 75-85% rule only if a third week of non-deployment proves the screen too strict.

### Overall Grade: D
- Risk-managed and rule-clean, but the core mission is to beat the S&P and we lagged it by 1.41% while sitting in cash through an up week. A disciplined loss is still a loss; chronic non-deployment is now the defining problem, not a one-off. Must actually deploy next week.

## Week ending 2026-06-26

### Stats
| Metric | Value |
|--------|-------|
| Starting portfolio | $99,198.93 (Mon 6/22 AM ≈ Fri 6/19 close) |
| Ending portfolio | $100,219.32 |
| Week return | +$1,020.39 (+1.03%) |
| S&P 500 week | +0.9% (holiday-shortened) |
| Bot vs S&P | +0.13% — NOMINAL ONLY; luck, not edge (see note) |
| Trades | 0 authorized (W:0 / L:0 / open:0). 9 unauthorized positions flattened (containment, not strategy) |
| Win rate | N/A (no authorized closed trades) |
| Best trade | N/A (no authorized trades) |
| Worst trade | N/A (no authorized trades) |
| Profit factor | N/A (no authorized trades) |

> NOTE on the +1.03% week: ZERO authorized strategy trades occurred. The entire gain is an accounting artifact of liquidating the attacker's 9 unauthorized positions (filled 6/24) into a green tape at the 6/25 open (+$755.62 realized). The bot earned none of this; it could as easily have been a loss. Real strategy P&L this week = $0. The "beat" vs S&P is noise.

### Closed Trades
| Ticker | Entry | Exit | P&L | Notes |
| — | — | — | — | No AUTHORIZED trades closed this week |
| AAPL/AMD/AVGO/INTC/MRVL/MSFT/MU/SNDK/TSLA | various (6/24) | 6/25 open | +$755.62 (aggregate) | UNAUTHORIZED — attacker-opened, flattened as containment. Not strategy P&L. |

### Open Positions at Week End
| Ticker | Entry | Close | Unrealized | Stop |
| — | — | — | — | None — 100% cash, fully flat (0 positions, 0 open orders) |

### What Worked
- Incident response was the week's only real work, and it was executed well: caught and cancelled 4 overnight rogue buy batches before fill; on 6/24 when 9 rogue lots DID fill naked, flattened them at the next open and drove long MV to $0 despite the paper engine throttling the sells.
- Never knowingly carried unauthorized exposure past a session under my control; honored the no-naked-risk rule throughout. By Friday close the book was flat for the 2nd straight day with the 5th rogue batch (10 orders) cancelled pre-open before any fill.
- Zero authorized rule violations: 0/3 weekly trades, 0/6 positions, daytrade_count 0, PDT false all week.
- Correctly refused to deploy authorized capital on top of a compromised key — security override was the right call.

### What Didn't Work
- THE STRATEGY DID NOT TRADE — third consecutive week with no authorized deployment. Two weeks it was an over-restrictive screen; this week a (justified) security halt. Either way the mission engine has been idle for ~3 weeks.
- The security incident is UNRESOLVED on Day 5. The bot has alerted the user to rotate ALPACA_API_KEY/SECRET every session since 6/22; the key has NOT been rotated. Containment depends entirely on the pre-market run catching each overnight batch — one missed run = naked fills again (proven 6/24). This is the dominant, escalating risk.
- The headline +1.03% is luck from an attacker's lucky liquidation, not edge. Presenting it as a "win" would be self-deception; flagged explicitly so it doesn't pollute the phase record.
- Phase P&L (+$219.32 / +0.22% vs $100k) is likewise an artifact of the 6/25 green flatten, not strategy performance. The strategy's own realized record remains -$801.07 (the XLE loss), 0-for-1 closed.

### Key Lessons
- A persistent credential compromise is an operational emergency that the bot alone cannot fix — it can only contain. When the only mitigation is a user action (key rotation) and the user hasn't acted in 5 days, daily in-band alerts are not landing. Escalation must be louder and clearer, not just repeated.
- Cancel-each-morning containment is fragile by design: it is a race against the open and has already failed once (6/24 fills). It is NOT a substitute for rotating the key, and the review must say so plainly rather than reporting "contained" as if resolved.
- Three weeks of a near-flat book means the challenge clock is running with the strategy on the sidelines. The opportunity cost is now structural, but it cannot be addressed until the account is secure — security strictly precedes any deployment-floor discipline.

### Adjustments for Next Week
- NO authorized trading resumes until the user rotates ALPACA_API_KEY/SECRET and confirms the account is clean. This is non-negotiable and overrides any deployment-floor or tape signal.
- Every session next week: pre-market run MUST cancel any fresh rogue injection before the open and verify the book is flat; market-open/midday/EOD re-verify. Treat a missed pre-market run as the top operational risk.
- The moment the key is confirmed rotated/clean: resume the normal screen and begin redeploying toward 75-85% on a confirmed, single-name momentum leg (Industrials/Materials favored on the 2026 rotation; energy stays OFF with WTI <$70; treat the Micron/AI-semis pop as a counter-trend bounce against hot PCE 4.1% + ~80% Sep-hike odds + VIX 21).
- No strategy hard-rule change this week. The framework is not the problem — an unresolved compromise is. Re-evaluate the screen/deployment rules only after security is restored and the strategy has a clean week to actually trade.

### Overall Grade: D
- Containment was handled competently, but the core mission — trade to beat the S&P — did not happen for a third straight week, and a critical security incident the bot has flagged for 5 days remains unfixed because it requires a user action that hasn't occurred. The +1.03% is luck, not edge. A well-run holding pattern on a compromised account is still a non-performing week; the only path off this grade is the user rotating the key so the strategy can resume.
