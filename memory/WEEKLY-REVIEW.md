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
