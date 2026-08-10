# MORSECORP Inc - A Compliance Failure Case Study
### Analyzing the $4.6M False Claims Act Settlement Through a GRC Lens

**Focus Areas:** Governance, Risk & Compliance (GRC) · Federal Compliance Frameworks · Access Control

**Case Basis:** United States ex rel. Berich v. MORSECORP Inc. et al., No. 23-cv-10130 (D. Mass.) 

---

## 1. Summary

In March 2025, the Department of Justice announced a **$4.6 million False Claims Act settlement** with MORSECORP Inc. (MORSE), a Cambridge, Massachusetts defense contractor working with the Departments of the Army and Air Force. The case wasn't about a data breach (no hack is alleged). It was about **falsely certifying cybersecurity compliance** to keep collecting government payments while knowingly failing to meet the security requirements those contracts required.

This case study treats MORSE's admitted facts as source material for a compliance gap analysis: what specifically failed, how it maps to the NIST SP 800-171 control families, and what a GRC program should have caught before it became a $4.6 million legal problem. Every finding here is drawn from facts MORSE itself admitted, acknowledged, and accepted responsibility for as part of the settlement.

## 2. What MORSE Admitted To (Source: DOJ Settlement)

The settlement lists four specific admitted failures, spanning January 2018 to June 2023:

1. **Unvetted third-party email hosting (Jan 2018 – Sept 2022):** MORSE used a third-party company to host its email without requiring or verifying that the vendor met security requirements equivalent to the FedRAMP Moderate baseline, or complied with DoD requirements for cyber incident reporting, malicious software handling, and forensic evidence preservation.
2. **Incomplete NIST SP 800-171 implementation (Jan 2018 – Feb 2023):** MORSE's contracts required full implementation of all NIST 800-171 controls. MORSE had not fully implemented them including controls whose absence could allow significant network exploitation or exfiltration of controlled defense information.
3. **No System Security Plan (Jan 2018 – Jan 2021):** Despite a contractual requirement, MORSE had no consolidated written plan describing its system boundaries, operating environment, how security requirements were implemented, or connections to other systems.
4. **Falsified and unreported compliance score (Jan 2021 – June 2023):** MORSE self reported a NIST 800-171 implementation score of **104** (near the top of the possible range, which runs from -203 to 110) to the DoD's scoring system (SPRS) in January 2021. In July 2022, an independent third-party cybersecurity consultant assessed MORSE's actual score at **-142**. MORSE did not correct its official score until **June 2023, three months after being served a federal subpoena**

## 3. Mapping the Failures to NIST 800-171 Control Families

| Admitted Failure | Control Family | Why It Matters |
|---|---|---|
| Unvetted third-party email vendor | **System & Communications Protection (SC)** / Supply Chain | MORSE extended trust to a vendor without validating that vendor met an equivalent security baseline creating a third-party risk failure|
| Incomplete 800-171 implementation | **Multiple (spans nearly all 14 families)** | This wasn't one missed control it was a program wide failure to implement the baseline the contract required |
| No System Security Plan | **Program-level documentation requirement** | The SSP is the foundational document that proves *how* controls are implemented. Without it, there's no audit trail nothing to show an assessor, and arguably nothing forcing internal accountability either |
| False SPRS score, uncorrected for 11 months post-discovery | **Governance / Integrity of Reporting** | This is the most damaging failure from a legal standpoint converting a compliance gap (bad, but common) into a **known false certification** (a legal liability under the False Claims Act) |

## 4. The Critical Distinction: Non-Compliance vs. False Certification

This is the single most important lesson this case teaches, and it's one every GRC analyst needs to internalize:

**Being non-compliant is a business risk. Knowingly certifying that you're compliant when you're not is a legal one.**

MORSE's exposure wasn't primarily about having a -142 score instead of a 104. Plenty of defense contractors have real gaps and manage them through a documented POA&M. What triggered False Claims Act liability was:

- Learning the true score in **July 2022**
- Not correcting the official DoD record until **June 2023**
- Only doing so **after being subpoenaed**, not proactively

That eleven-month gap between *knowing* and *disclosing* is where a compliance gap became a fraud allegation. A POA&M with an honest -142 score and a remediation plan is a normal, defensible compliance posture. A stale, known-false 104 score sitting in a federal system while the company kept collecting payment is not.

## 5. What a Functioning GRC Program Would Have Caught

Working backward from the DOJ's findings, here's where structured governance would have intervened:

- **A vendor risk management process** would have required the email hosting provider to demonstrate FedRAMP Moderate equivalency *before* onboarding — not left it unverified for four years.
- **A living SSP**, reviewed and updated on a defined cadence, would have made the compliance gap visible internally well before an external consultant found it in 2022.
- **A defined score-update policy** — tying any material change in assessed maturity to a mandatory SPRS resubmission window (e.g., 30 days) — would have prevented an eleven-month lag between discovery and correction.
- **An escalation path** ensuring that a finding this severe (a swing of nearly 250 points on the SPRS scale) reaches legal and executive leadership immediately, given the False Claims Act exposure of an uncorrected federal certification.

## 6. Scope Exclusions & Where This Analysis Breaks Down

**Excluded from this analysis, and why:**
- **MORSE's internal decision-making process** — the DOJ settlement documents *what* MORSE admitted, not *why* internal stakeholders chose not to correct the score for 11 months. Any explanation here would be speculation the public record doesn't support.
- **Full technical remediation detail** — the settlement doesn't disclose which specific 800-171 controls were unmet beyond the general narrative; a control-by-control breakdown here would be fabricated, not sourced.
- **Criminal liability** — this was a *civil* False Claims Act settlement. This case study doesn't address whether any individual faced or could have faced criminal exposure, which is a separate legal question outside GRC scope.

**Where this analysis is weakest:**
- This is a retrospective analysis built entirely from a public settlement announcement, not an internal audit — it necessarily reflects only what the government chose to include in the public record, not the complete factual picture.
- The "what a functioning GRC program would have caught" section in Section 5 is my own reasoned inference from the facts, not confirmed by MORSE — a rigorous reviewer should treat it as informed analysis, not documented fact.
- There's a real risk of hindsight bias here — it's easy to say "a review cadence would have caught this" after the fact. A fair critique: plenty of companies have SSP review cadences and vendor risk programs that still miss things. The real differentiator in this case wasn't the absence of *any* process — it was the 11-month gap between knowing and disclosing, which is a leadership/integrity failure more than a pure process failure.

## 7. TLTR

*"A defense contractor called MORSE told the government it was following the cybersecurity rules and hosting sensitive data securely, filing the right paperwork. While collecting payment on Army and Air Force contracts. It wasn't. Worse, when an outside consultant told them in mid-2022 that their actual compliance score was nowhere close to what they'd reported, they sat on that information for almost a year, and only fixed the record after the government subpoenaed them. That's not a technical mistake anymore it turned into a lawsuit costing them $4.6 million, and why the whistleblower who reported it. MORSE's own security officer got a $851,000 cut of the settlement."* (smart guy)

## 8. What This Case Study Demonstrates

- Ability to analyze a real regulatory enforcement action and extract actionable GRC lessons
- Understanding of the legal distinction between compliance gaps and false certification

---
*This case study is built entirely from publicly available Department of Justice materials, specifically the March 26, 2025 press release and settlement agreement in United States ex rel. Berich v. MORSECORP Inc. et al. All quoted facts are matters of public record; analysis and interpretation beyond the admitted facts are clearly identified as such in Sections 5 and 6.*
