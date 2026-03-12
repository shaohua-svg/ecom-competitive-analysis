# ecom-competitive-analysis

> E-Commerce Competitive Analysis Skill v3.0 for Claude (Cowork / Claude Code)

Given a product URL, this skill runs a full competitive analysis workflow and produces a structured, actionable report that directly supports ad launch decisions.

## What It Does

1. **Extracts product data** from any e-commerce URL (Amazon, Shopify, Etsy, etc.)
2. **Discovers competitors** via 6 parallel channels (platform search, Google, Ad Library, SimilarWeb similar sites, keyword reverse-lookup, user-specified)
3. **Collects real audience data** from SimilarWeb (age, gender, traffic sources) — no guesswork
4. **Generates a 3-part report**:
   - One-page decision brief (read in 2 minutes, act immediately)
   - Competitor overview cards + comparison table
   - Deep 4-module analysis with credibility ratings

## v3.0 Highlights

- **SimilarWeb integration** — real audience demographics replace pure inference
- **Three-layer data architecture** — Auto → User Input → Paid Test
- **Three-layer audience model** — Influencer / Buyer / User layers
- **Ad group design based on real data** — 5 ad groups mapped to actual audience
- **"Don't do" recommendations** — helps avoid wasting budget

## Installation

### Claude Code
```bash
git clone https://github.com/shaohua-svg/ecom-competitive-analysis.git
cp -r ecom-competitive-analysis/ecom-competitive-analysis ~/.claude/skills/
```

### Cowork Mode
Download the `.skill` file from [Releases](../../releases) and install it in Cowork.

### ClawHub
```bash
clawhub install ecom-competitive-analysis
```

## Usage

Simply provide a product URL to Claude:
```
"Help me analyze competitors for this product: https://example.com/product-url"
```

Or use trigger phrases: "竞品分析", "competitive analysis", "find competitors", "listing优化", "投放策略"

## Example Output

See [examples/竞品分析报告v3_Shopping_Snow_Globe.md](examples/竞品分析报告v3_Shopping_Snow_Globe.md) for a full sample report.

## Credibility System

| Rating | Meaning | Verification Cost |
|--------|---------|-------------------|
| ★★★★★ | Page-extracted fact / first-party data | None |
| ★★★★☆ | Authoritative third-party + light inference | Low |
| ★★★☆☆ | Multi-source cross-inference | $20-50 test |
| ★★☆☆☆ | Industry data + estimation | 1-2 weeks |
| ★☆☆☆☆ | Limited-info speculation | Cannot verify |

## License

MIT License — see [LICENSE](LICENSE)
