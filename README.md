# US Tenbagger Stock Picker

**English** · [简体中文](README.zh-CN.md)

“Could this become ten times larger?” is the opening question. The interesting part is showing your work.

```mermaid
flowchart LR
  A[Candidate company] --> B[Ten-factor research scorecard]
  B --> C[Per-share compounding thesis]
  C --> D[Metrics and thesis breakers]
```

A Codex skill for analyzing possible US tenbagger stocks.

This skill combines two ideas:

- A factor-based tenbagger screen: small starting market cap, valuation mismatch, profitability, free cash flow, reinvestment quality, momentum behavior, and macro liquidity.
- A structural compounding framework: FCF-per-share inflection, Costco-style shared-scale models, and NVDA-style technology-breakthrough models.

This is a research workflow, not investment advice.

## What This Skill Does

Use this skill when you want Codex to evaluate whether a US-listed company has the ingredients of a long-term multibagger.

It helps answer:

- Can this company plausibly become much larger?
- Is the market misunderstanding the business?
- Is free cash flow per share improving?
- Is growth compounding per share, or being diluted away?
- Does the company fit a Costco-style or NVDA-style compounding model?
- What data would confirm or break the thesis?

## Installation

Copy the folder into your local Codex skills directory:

```bash
mkdir -p ~/.codex/skills/us-tenbagger-stock-picker
cp SKILL.md ~/.codex/skills/us-tenbagger-stock-picker/SKILL.md
```

Then ask Codex to use the skill:

```text
Use us-tenbagger-stock-picker to analyze HIMS as a possible tenbagger.
```

## Recommended Prompts

Quick screen:

```text
Use us-tenbagger-stock-picker to quickly screen TICKER as a possible tenbagger.
```

Deep research:

```text
Use us-tenbagger-stock-picker to deeply analyze TICKER. Include scorecard, model classification, metrics to verify, and thesis breakers.
```

Comparison:

```text
Use us-tenbagger-stock-picker to compare TICKER_A and TICKER_B as tenbagger candidates.
```

Watchlist:

```text
Use us-tenbagger-stock-picker to build a watchlist of US small-cap companies that may fit the Costco or NVDA model.
```

## Framework Summary

A strong tenbagger candidate usually combines:

```text
Low starting base
+ improving business quality
+ free cash flow inflection
+ long reinvestment runway
+ structural growth driver
+ market under-recognition
+ favorable or improving liquidity cycle
```

The skill scores ten categories from 0 to 3:

| Factor | What It Tests |
| --- | --- |
| Small starting market cap | Whether the company has enough room to compound |
| Valuation mismatch | Whether the market is mispricing or misclassifying the business |
| Profitability quality | Whether growth is becoming economically valuable |
| FCF per share inflection | Whether each share has a growing claim on future cash flow |
| Reinvestment quality | Whether spending creates durable future returns |
| Costco model fit | Whether scale improves value for customers and deepens trust |
| NVDA model fit | Whether long technical accumulation can unlock explosive value |
| Data or AI flywheel | Whether users, usage, data, and product quality compound |
| Momentum and drawdown | Whether price action is strong but still thesis-supported |
| Macro liquidity | Whether rates and liquidity support long-duration growth |

## Output Structure

The skill produces:

- Tenbagger thesis
- Scorecard
- Model classification
- What the market may be missing
- Key metrics to verify
- Thesis breakers
- Verdict

See [examples/hims-example.md](examples/hims-example.md) for an example output.

## Important Limitations

- The skill does not replace financial statements, filings, or current market data.
- It should not be used as a standalone buy or sell signal.
- Scores are research aids, not predictions.
- Current data must be verified before making any investment decision.
- Many tenbagger candidates will fail, dilute shareholders, or suffer large drawdowns.

## Final Test

A real tenbagger thesis must answer:

```text
Why can this company become much larger?
Why has the market not fully priced it in?
Why will per-share value compound instead of being diluted away?
```

If those questions cannot be answered clearly, the stock is not yet a high-quality tenbagger candidate.
