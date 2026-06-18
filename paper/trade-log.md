# Paper Trade Log — Simulation Start 2026-06-12

> All prices are simulated fills. 0.1% slippage applied to every entry and exit.
> Universe: AMD, AVGO, SMCI, MU, MRVL, META, VST, UBER, CCJ, GOOGL, AMZN, MSFT, AAPL, NFLX, JPM, V, BRK.B, COST, WMT, LLY, XOM
> Max position: 25% of $1,000 starting capital = $250. Max 4 open positions. Long only.

---

## 2026-06-12 (Day 1)

| # | Symbol | Action | Shares | Fill Price | Gross | Slippage | Net Cost | Source / Timestamp |
|---|--------|--------|--------|------------|-------|----------|----------|--------------------|
| 1 | AMD    | BUY    | 0.4852 | $515.31    | $249.97 | $0.25  | $249.97  | StocksToTrade / FinancialContent, June 12 2026 ~market close; raw quote $514.80 × 1.001 |

**Passed on second slot:** UBER ($68.48) showed relative weakness vs SPY (+1.7%) — trading near its 52-week low of $67.19 despite a broad risk-on rally. No clear catalyst. MRVL already up 70.6% in June — chasing extension. Holding cash for better setups days 2–4.

---

## 2026-06-15 (Day 2)

> Continuity note: state was found on branch `claude/modest-ride-chjabw` (no `main` branch exists; prior runs each reset to a fresh Day 1 on separate branches). This run continues the 06-12 state as Day 2 without resetting.

| # | Symbol | Action | Shares | Fill Price | Gross | Slippage | Net Cost | Source / Timestamp |
|---|--------|--------|--------|------------|-------|----------|----------|--------------------|
| 2 | VST    | BUY    | 1.6140 | $154.87    | $249.72 | $0.25  | $249.97  | Google Finance / stockanalysis, June 15 2026 ~15:20 ET; raw quote $154.72 × 1.001 |
| 3 | MRVL   | BUY    | 0.8600 | $290.60    | $249.67 | $0.25  | $249.92  | GuruFocus / Yahoo Finance, June 15 2026; raw quote $290.31 × 1.001 |

**HOLD:** AMD — current $515.92 vs avg cost $515.31 (+0.12%); well clear of stop $489.54 and target $570. Citi-upgrade + UK-AI-investment thesis intact; sector strong. No action.

**Passed:** XOM — US-Iran peace deal reopened the Strait of Hormuz and oil fell to ~$80 (from ~$96), killing the oil-supply-shock thesis that drove prior XOM consideration. UBER — still no catalyst. META — China (Manus unwind) + EU regulatory overhang unresolved.

**Cash after Day 2:** $250.14 (4th slot left open intentionally as a buffer given AMD+MRVL semiconductor correlation).

---

## 2026-06-16 (Day 3)

> Continuity: restored full Day-2 state from branch `claude/sharp-hawking-kpz1jk` and continued without resetting. Committed to harness-assigned branch `claude/sharp-hawking-fnb78g` (no `main` exists; pushing elsewhere not permitted). Short week: Day 5 (close-all) = Thu 06-18 (Fri 06-19 = Juneteenth holiday).

**NO NEW TRADES.** No buys, no sells. One position adjustment (stop raise) below.

| Symbol | Action | Detail | Source / Timestamp |
|--------|--------|--------|--------------------|
| AMD | RAISE STOP | $489.54 → $520.00 (trailing; below today's intraday low ~$530.14, locks ≈+0.9% vs $515.31 entry) | CNBC/Yahoo, AMD $538.74 on June 16 2026 (−1.56%, ATH $547.26 set 06-15) |

**HOLD AMD** — $538.74 (+4.5% vs $515.31). Just off all-time high; Citi-upgrade/AI-demand thesis intact. Far below new $520 stop-risk and approaching $570 target. Raised stop to protect the gain into the last two sessions.

**HOLD VST** — ~$154.72 (06-16 quote lagging; ~flat vs $154.87 entry). AI-power thesis intact; held original $147.13 stop.

**HOLD MRVL** — ~$296.50 (+2.0% vs $290.60; pulled back ~4% from the $308.88 Day-2 close). Red flags noted: CFO Willem Meintjes resigned effective 06-15, the outgoing CFO filed to sell ~$65M of shares, and "chip momentum snapped" on a soft tape (INTC recession warning). The S&P 500 index-inclusion catalyst (06-22) is mechanically unchanged but lands AFTER this run's Day-5 close. Still +2% and well above the $276.07 stop, so held; stop NOT tightened because ~$288 would risk a noise stop-out (today's low ≈ $288). Monitoring closely for a momentum break.

**Passed on 4th slot:** GOOGL (+2.5% on tech-earnings focus) and UBER (+2.8% on California collision-insurance cost cuts) both had fresh same-day catalysts, but with only two sessions left (Day 4 06-17, Day 5 06-18) a new entry has minimal runway, the tape is nervous on tariff fears, and slippage is a guaranteed cost. Kept the 4th slot open and $250.14 in cash as a buffer against AMD+MRVL semiconductor correlation. "No trade" is the disciplined call this late in the window.

**Cash after Day 3:** $250.14 (unchanged).

---

## 2026-06-17 (Day 4)

> Continuity: restored full Day-3 state from branch `claude/sharp-hawking-fnb78g` and continued without resetting. Committed to harness-assigned branch `claude/sharp-hawking-jmolam` (no `main` exists; pushing elsewhere not permitted). Day 5 (close-all) = Thu 06-18.

**RISK FIRST — two exits processed before any entry consideration. Risk-off, semiconductor-correction day.**

| # | Symbol | Action | Shares | Fill Price | Gross | Slippage | Net Proceeds | Source / Timestamp |
|---|--------|--------|--------|------------|-------|----------|--------------|--------------------|
| 4 | AMD  | SELL (STOP) | 0.4852 | $519.48 | $252.05 | $0.25 | $252.05 | Stop $520.00 × 0.999. AMD 06-17 intraday low ~$507.25 / prev close ~$507.29 (stockanalysis/Yahoo via search); opened $520.92, rebounded to +4.5% on Rackspace deal |
| 5 | MRVL | SELL (THESIS) | 0.8600 | $278.39 | $239.42 | $0.24 | $239.42 | Market $278.67 × 0.999; Yahoo/Google Finance, June 17 2026 (−9.8% from $308.88 prev close; day range $278.13–$317.00) |

**AMD — STOP HIT.** Stop was $520.00 (raised Day 3). On 06-17 AMD traded below it (intraday low ~$507.25, prev close ~$507.29) before a dip-buying rebound to +4.5% on the AMD–Rackspace 30MW AI-compute deal and a Bernstein PT raise to $600. A stop is non-discretionary, so I exited at $520.00 (−0.1% slip → $519.48). Realized **+$2.02 (+0.81%)** — a small win and disciplined protection against the intraday plunge to $507. Honoring the stop cost some of the late rebound, but cherry-picking around a stop is not how this sim is run.

**MRVL — THESIS BROKEN, exited above stop.** MRVL fell ~9.8% to $278.67 (day low $278.13, just above the $276.07 stop) in a broad semiconductor selloff (SOXX −5.92% on 06-16). This is a decisive break below its recent range, on top of the 06-15 CFO resignation and the ~$65M outgoing-CFO insider sale. The only remaining bull case — mechanical S&P 500 index inclusion — lands 06-22, *after* the Day-5 close, so it cannot help within the window. Per the hard rule ("exit if a thesis is broken by news, even if the stop isn't hit") and my own Day-3 plan ("exit on a decisive break below the recent range… do not wait for the 06-22 catalyst"), I sold at market $278.39. Realized **−$10.50 (−4.20%)** — cut before the stop and before likely further downside.

**HOLD VST** — ~$161 (range $157.60–$163.53, open $158.84; Yahoo/Google Finance 06-17). +3.9% vs $154.87 entry and showing relative strength on a risk-off day while semis sold off — the diversification thesis working. Stop **RAISED $147.13 → $155.00** (just above breakeven) to lock in a non-loss against an overnight gap into the Day-5 forced close. Target $175.

**NEW ENTRIES: NONE (0 of up-to-2).** Day 4 of 5 on a risk-off tape with semiconductors in a sharp correction and only one session of runway before the forced Day-5 liquidation. A new entry guarantees ~0.2% round-trip slippage for minimal time to work; re-entering AMD right after a stop-out would be chasing. The disciplined call is to bank the AMD win, cut the MRVL loser, hold the VST winner, and carry a large cash buffer ($741.61) into the close.

**Cash after Day 4:** $741.61 ($250.14 + $252.05 AMD + $239.42 MRVL).

---

## 2026-06-18 (Day 5 — FINAL, FORCED CLOSE-ALL)

> Continuity: restored full Day-4 state from branch `claude/sharp-hawking-jmolam` and continued without resetting (starting capital $1,000, full history, SPY baseline $737.76 all preserved). Committed to harness-assigned branch `claude/sharp-hawking-9pc40s` (no `main` exists; pushing elsewhere not permitted). This is the final session — all positions liquidated.

**RISK CHECK FIRST.** Only one open position remained: VST. It traded $157.30–$162.40 on 06-18 (~$160.40 last; Yahoo/Google Finance), well above its $155.00 stop and below the $175 target — neither hit. Thesis fully intact (KKR-led $10B Helix Digital Infrastructure AI-power venture named VST anchor investor/preferred power provider on 06-11; Meta/AWS PPAs; analyst median PT ~$232). No stop/target/thesis trigger — so the close is purely the Day-5 mandatory liquidation, not a risk exit.

| # | Symbol | Action | Shares | Fill Price | Gross | Slippage | Net Proceeds | Source / Timestamp |
|---|--------|--------|--------|------------|-------|----------|--------------|--------------------|
| 6 | VST | SELL (DAY-5 CLOSE) | 1.6140 | $160.24 | $258.63 | $0.26 | $258.63 | Raw quote $160.40 × 0.999 slip; Yahoo/Google Finance, June 18 2026 (range $157.30–$162.40) |

**VST — CLOSED @ $160.24 (raw $160.40 − 0.1% slip). Realized +$8.67 (+3.47%).**
The diversifier delivered. VST was added on Day 2 specifically as a non-semiconductor AI-demand name, and it earned its place: while AMD and MRVL were hit by the 06-16/06-17 chip correction (SOXX −5.92%), VST held relative strength on AI-electricity demand and finished as the book's best trade. Sold only because the simulation window closed; thesis remained intact.

**NEW ENTRIES: NONE.** Day 5 is liquidation-only — no new positions on the final session.

**Cash after Day 5:** $1,000.24 ($741.61 + $258.63 VST). **All positions flat — simulation complete.**

---

## Final Realized P&L Summary

| Trade | Entry → Exit | Realized $ | Realized % | Result |
|-------|--------------|-----------|-----------|--------|
| AMD  | $515.31 → $519.48 (stop) | +$2.02 | +0.81% | Win |
| MRVL | $290.60 → $278.39 (thesis broken) | −$10.50 | −4.20% | Loss |
| VST  | $154.87 → $160.24 (Day-5 close) | +$8.67 | +3.47% | Win |
| **Total** | | **+$0.19** | | **2 wins / 1 loss** |

- **Final portfolio value:** $1,000.24 (100% cash) — **+$0.24 / +0.02%** vs $1,000 start (the $0.05 gap vs the +$0.19 line sum is avg-cost-vs-net-cost rounding across fills).
- **Win rate:** 66.7% (2 of 3 closed trades).
- **Best trade:** VST +$8.67 (+3.47%). **Worst trade:** MRVL −$10.50 (−4.20%).
- **Benchmark:** SPY $737.76 (Day-1 baseline) → ~$753.50 (06-18) = **+2.13%**. Portfolio +0.02% **trailed SPY by ~2.1 pts.**
