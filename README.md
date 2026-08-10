# MORSECORP Inc.: A Real-World Compliance Failure Case Study

Analysis of the $4.6M False Claims Act settlement between the Department of Justice and defense contractor MORSECORP Inc. — read through a GRC (Governance, Risk & Compliance) lens, mapped to NIST SP 800-171, and built to demonstrate applied compliance judgment rather than framework recitation.

**Author:** Antonio Talavera
**Focus Areas:** Governance, Risk & Compliance (GRC) · Federal Compliance Frameworks · Access Control
**Case Basis:** *United States ex rel. Berich v. MORSECORP Inc. et al.*, No. 23-cv-10130 (D. Mass.) — DOJ settlement announced March 26, 2025

---

## Why This Project Exists

Most portfolio pieces in this space explain what a compliance framework *says*. This one instead asks: what happens when a real company gets it wrong, and what specifically turns "we have compliance gaps" into a $4.6 million federal fraud settlement?

Every fact below is drawn from what MORSECORP itself admitted, acknowledged, and accepted responsibility for as part of its DOJ settlement — not a hypothetical scenario.

## What MORSE Admitted To

Spanning January 2018 to June 2023, MORSE admitted to four specific failures:

1. **Unvetted third-party email hosting** (Jan 2018 – Sept 2022) — used a third-party provider to host company email without verifying it met a FedRAMP Moderate–equivalent security baseline or DoD cyber incident reporting requirements.
2. **Incomplete NIST SP 800-171 implementation** (Jan 2018 – Feb 2023) — contracts required full implementation of all NIST 800-171 controls; MORSE had not fully implemented them, including controls whose absence could enable significant network exploitation or exfiltration of controlled defense information.
3. **No System Security Plan** (Jan 2018 – Jan 2021) — no consolidated written plan describing system boundaries, operating environment, or how security requirements were implemented, despite a contractual requirement to maintain one.
4. **Falsified and unreported compliance score** (Jan 2021 – June 2023) — self-reported a NIST 800-171 score of **104** (near the top of the -203 to 110 range) in January 2021. An independent consultant found the actual score was **-142** in July 2022. MORSE didn't correct the official record until **June 2023 — three months after being federally subpoenaed.**

## The Core Lesson

**Being non-compliant is a business risk. Knowingly certifying compliance you don't have is a legal one.**

MORSE's real exposure wasn't the -142 score itself — plenty of contractors carry real gaps, managed honestly through a documented POA&M. What created False Claims Act liability was the **eleven-month gap between learning the true score (July 2022) and correcting the federal record (June 2023)**, and doing so only after a subpoena forced the issue.

That distinction — compliance gap vs. false certification — is the single most important thing this case study is built to teach.

## What's In This Repo

| File | Contents |
|---|---|
| `morsecorp-compliance-case-study.md` | Full case study: admitted failures mapped to NIST 800-171 control families, the compliance-vs-fraud distinction, what a functioning GRC program would have caught, honest scope exclusions, and a 5-minute plain-language executive walkthrough |

## What This Project Demonstrates

- **Working from primary sources.** This analysis is built directly from the DOJ press release and settlement documents — not a secondary summary of the case.
- **Distinguishing compliance risk from legal risk.** Understanding *why* MORSE's failure became a fraud case, not just *that* it did, is the difference between reciting a framework and understanding how enforcement actually works.
- **Governance-level thinking, not just technical fixes.** The analysis identifies the missing *process* — a mandatory score-update policy, an escalation path to legal and executive leadership — not just the missing technical controls.
- **Intellectual honesty under self-scrutiny.** The case study explicitly separates public record from my own inference, and flags the risk of hindsight bias in its own reasoning — the kind of self-correction that matters when the job is telling leadership an uncomfortable truth.
- **Direct relevance to defense-adjacent employers.** This is precisely the enforcement environment that shapes supply chain compliance requirements for companies like Boeing and their subcontractor networks.

## The One-Line Summary

*I don't just know what NIST 800-171 requires — I can point to a company that got fined $4.6 million for the specific governance failure of knowing they weren't compliant and not saying so, and I can explain exactly what would have stopped it.*

---
*This case study is built entirely from publicly available Department of Justice materials — specifically the March 26, 2025 press release and settlement agreement in United States ex rel. Berich v. MORSECORP Inc. et al. All admitted facts are matters of public record; analysis and interpretation beyond those facts are clearly identified as such within the case study.*
