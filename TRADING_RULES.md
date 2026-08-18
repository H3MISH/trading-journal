# Automated Trading Rules

Binding constraints for any agent session that proposes or places trades on this account.
These are not suggestions. If a rule blocks a trade, the trade does not happen.

## Account

- **Only account:** `628884785` ("Agentic", cash, `agentic_allowed=true`)
- **Never touch** account `508245164` (margin, ••4164). No orders, no position changes, ever.

## Instruments

- Equities only.
- No options. No crypto. No margin.

## Sizing

- **Max $50 risked per trade proposal.** Risk = full position cost for an equity buy
  (a stock can go to zero), not a stop-distance calculation.
- One open proposal at a time. Do not stack proposals while one is pending approval.

## Approval — the hard gate

- **No order is ever placed without explicit human approval of that specific trade.**
- The agent proposes: ticker, side, dollar size, entry, thesis, and what would make it wrong.
- The human replies approve/reject. Only on approval does the agent call `place_equity_order`.
- Silence is not approval. An expired or unanswered proposal is dead — re-propose next session.
- No standing authorization. Approving one trade authorizes exactly that trade.

## Circuit breakers

- If account value drops below **$150** (25% drawdown from the $200 starting balance),
  stop proposing trades and report the drawdown instead.
- Three consecutive losing closed trades → pause proposals, write a post-mortem first.

## Journaling

Every proposal and every fill gets an entry in `journal/`. An entry records:
thesis, size, risk, outcome, and what was learned. A trade with no journal entry
did not happen correctly, regardless of its P&L.

## Why these limits exist

The ••4164 margin account's history (19 months, ~340 closed trades) shows +1.28% total
rate of return on +$6,408 realized P&L, with monthly swings from -80.7% to +70.0% and
multiple -100% single-position option losses. That is a sizing and discipline problem,
not a thesis problem. These rules exist to prove process on small size before size
is ever the question.
