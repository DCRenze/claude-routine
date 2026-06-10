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

---

## Week ending 2026-06-10

### Stats
| Metric | Value |
|--------|-------|
| Starting portfolio | $100,000.00 (working baseline) |
| Ending portfolio | $100,000.00 |
| Week return | $0.00 (0.0%) |
| S&P 500 week | -2.6% (FRED weekly, wk ending Jun 5) |
| Bot vs S&P | +2.6% (flat cash vs declining index) |
| Trades | 0 (W:0 / L:0 / open:0) |
| Win rate | N/A (no closed trades) |
| Best trade | None |
| Worst trade | None |
| Profit factor | N/A |

### Closed Trades
| Ticker | Entry | Exit | P&L | Notes |
| — | — | — | — | No trades this week |

### Open Positions at Week End
| Ticker | Entry | Close | Unrealized | Stop |
| — | — | — | — | None — 100% cash |

### What Worked
- Account came online and verified ACTIVE; API wrappers, env, and data feeds all functional.
- No capital lost during a down week (-2.6% S&P) — sat in cash by default rather than forcing a trade with no researched edge.
- Funding mismatch caught and flagged early (Alpaca equity $100k vs $10k baseline).

### What Didn't Work
- Zero capital deployed — strategy targets 75-85% deployed; bot is at 0%.
- No pre-market research log entries yet, so no vetted trade ideas to act on.
- Only one session (Day 1) inside this review window — not a full trading week.

### Key Lessons
- Cold-start week: infrastructure validated but no trading engine activity. Next week is the real test of execution discipline.
- Baseline must be confirmed with user. Treating $100k as working baseline; all Phase/return math anchors here until corrected.
- Outperforming S&P by being flat is luck, not skill — not a repeatable edge.

### Adjustments for Next Week
- Run pre-market research daily and populate RESEARCH-LOG.md before any trade.
- Begin deploying toward the 75-85% target as researched setups appear; respect max 3 new trades/week.
- Confirm $100k baseline with user before next weekly review.
- No strategy rule changes — insufficient data (0 trades) to justify any change.

### Overall Grade: C
