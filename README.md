# International Financial Law Practitioner

An Agent Skill that turns an agent into a structured international-financial-law practitioner across transactions, markets and regulation, international financial institutions, sovereign risk, trade finance, FinTech, and financial-data governance.

It distills fifteen books, chapters, and articles into four working layers: transaction architecture; markets, prudential regulation, and internal governance; IFIs, sovereign risk, and soft law; and FinTech, data governance, and regulatory trade-offs.

## Layout

```text
SKILL.md                  # expert reasoning core + task-based loading triggers (always loaded)
references/
  reference-<slug>.md     # one dense, standalone distillation per source (loaded on demand)
```

`SKILL.md` is the only file an agent loads automatically. Its first-person core establishes transaction judgment; the final Loading depth table selects source modules only when relevant.

## Sources

### Transactions & trade finance
| Source | Distillation |
|---|---|
| **Law and Practice of International Finance** — Philip R. Wood | [`reference-wood-international-finance.md`](references/reference-wood-international-finance.md) |
| **The Handbook of International Trade and Finance** — Anders Grath | [`reference-grath-trade-finance.md`](references/reference-grath-trade-finance.md) |
| **Leasing in Development** — Matthew Fletcher, Rachel Freeman, Murat Sultanov & Umed Temirbek | [`reference-fletcher-leasing-development.md`](references/reference-fletcher-leasing-development.md) |

### Markets, prudential regulation & internal governance
| Source | Distillation |
|---|---|
| **International Finance: Transactions, Policy, and Regulation** — Hal S. Scott & Anna Gelpern | [`reference-scott-gelpern-international-finance.md`](references/reference-scott-gelpern-international-finance.md) |
| **Banking Law and Regulation**, Chapters 5, 8 & 9 — Iris H-Y Chiu & Joanna Wilson | [`reference-chiu-wilson-prudential-regulation.md`](references/reference-chiu-wilson-prudential-regulation.md) |
| **Regulating (From) the Inside** — Iris H-Y Chiu | [`reference-chiu-internal-control.md`](references/reference-chiu-internal-control.md) |
| **Institutional Design: The Choices for National Systems** — Eilís Ferran | [`reference-ferran-institutional-design.md`](references/reference-ferran-institutional-design.md) |

### International institutions, sovereign risk & soft law
| Source | Distillation |
|---|---|
| **International Financial Institutions and International Law** — Daniel D. Bradlow & David B. Hunter (eds.) | [`reference-bradlow-hunter-ifis.md`](references/reference-bradlow-hunter-ifis.md) |
| **International Financial Law: Quo Vadis?** — Graeme Baber, selected chapters | [`reference-baber-quo-vadis.md`](references/reference-baber-quo-vadis.md) |
| **Why Soft Law Dominates International Finance—and Not Trade** — Chris Brummer | [`reference-brummer-soft-law.md`](references/reference-brummer-soft-law.md) |

### FinTech, data governance & regulatory trade-offs
| Source | Distillation |
|---|---|
| **Data Governance in AI, FinTech and LegalTech** — Joseph Lee & Aline Darbellay (eds.) | [`reference-lee-darbellay-data-governance.md`](references/reference-lee-darbellay-data-governance.md) |
| **Introduction—What Is FinTech?** — Jelena Madir | [`reference-madir-fintech-orientation.md`](references/reference-madir-fintech-orientation.md) |
| **Data Privacy in Mobile Payment** — Robin Hui Huang | [`reference-huang-china-mobile-payments.md`](references/reference-huang-china-mobile-payments.md) |
| **Fintech and the Innovation Trilemma** — Chris Brummer & Yesha Yadav | [`reference-brummer-yadav-innovation-trilemma.md`](references/reference-brummer-yadav-innovation-trilemma.md) |
| **Regulatory Agencies and the Inclusion Trilemma** — Chris Brummer | [`reference-brummer-inclusion-trilemma.md`](references/reference-brummer-inclusion-trilemma.md) |

## Install

Clone into the skill directory used by your agent. For Claude Code:

```bash
git clone https://github.com/ariel-lee-1023/iflaw-practitioner.git ~/.claude/skills/international-financial-law-practitioner
```

Other hosts use different roots, such as `~/.copilot/skills/`, `~/.agents/skills/`, `.claude/skills/`, or `.agents/skills/`. Keep the directory name `international-financial-law-practitioner` so it matches the `name:` in `SKILL.md`.

## Usage

```text
international-financial-law-practitioner
international-financial-law-practitioner about <transaction or issue>
international-financial-law-practitioner for <source>
```

Most substantial matters use two or three modules: one for transaction architecture, one for the applicable regulatory or institutional layer, and one specialist source.

## What kind of distillation this is

Structure, not chapter summaries. Each reference file states the source’s mental model, preserves named frameworks and legal distinctions, converts techniques into practitioner procedures, reconstructs one worked example, and ends with decision rules. The text is synthesized rather than copied at length.

The skill is deliberately strict about legal currency. It separates binding law, supervisory expectations, soft standards, market practice, contractual allocation, and analytical frameworks. It requires current primary-authority verification before operative advice and prevents China-, UK-, EU-, US-, or other jurisdiction-specific material from being generalized.

## Scope

Strong on cross-border loans and bonds, trade finance, guarantees and security, payment and securities-settlement systems, project and structured finance, prudential and systemic regulation, bank internal controls, IFI operations and accountability, sovereign debt, FinTech, data and AI governance, and regulatory design.

Important source limits:

- Wood combines the 1980 first edition with later-edition selected Chapters 7–12, 23–24, and 30.
- Baber includes the available Chapters 1, 2, and 5 rather than the full volume.
- Chiu & Wilson includes Chapters 5, 8, and 9.
- Lee & Darbellay prioritizes Chapters 1, 2, 4, 5, 6, 9, 10, and 11.
- Huang is a historical China-specific module.

For current rules, institutional mandates, sanctions, thresholds, or post-source reforms, the skill instructs the agent to identify the gap, retrieve authoritative primary material, and mark the seam between library-based analysis and current-law research.

## Provenance

Built with [`Books-to-Skill-Refs`](https://github.com/ariel-lee-1023/Books-to-Skill-Refs). Scan-only sources were OCRed locally; logical chapter sets were consolidated before distillation. The library is checked with the project’s contract validator, cross-host skill validator, and strict injected-instruction scanner.

## License

[MIT](LICENSE) covers the original skill structure, expert core, loading guidance, README, and synthesized distillation text.

The underlying books and articles retain their own copyright and licensing terms and are not redistributed or relicensed here.
