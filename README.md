# FSD Wizard

A free, browser-based reference tool for Canadian Foreign Service officers and their families to understand NJC Foreign Service Directive (FSD) entitlements before and during a posting abroad.

**Live tool:** [fsd-wizard.vercel.app](https://fsd-wizard.vercel.app)

---

## What it does

Enter your posting profile — post city, salary, family situation, housing type, and tour details — and the tool generates a structured entitlement summary. The results page shows estimated annual allowances, a shelter contribution deduction (FSD 25), and an estimated net annual position.

## Covered areas

- Pre-posting: posting loan, relocation, household effects, vehicle shipping, principal residence
- At-post living: shelter cost, transportation, hardship allowances, post living allowance, family separation
- Family: spouse/CLP assistance, daycare, education allowances, education travel, special separation
- Health: preventive medical, health care expenses, health care travel, medical advance
- Financial allowances: FSP, PDA, PSA, PLA
- Leave and travel: post travel assistance, family reunion, compassionate travel, post leave option

## Key features

- Nothing is stored or transmitted — all calculations run locally in your browser
- All figures are traceable to NJC FSD source text (April 1, 2026 rates)
- Government of Canada (Canada.ca) visual design
- Post search auto-fills hardship level and unhealthy post status
- PSA / Post Leave election toggle (FSD 46) adjusts totals correctly
- PDA tour-weighted average for postings beyond 24 months (FSD 58)
- Shelter contribution deduction (FSD 25, Appendix A) based on salary and household size
- Daycare section enables automatically when children under 6 are entered

## How to use

1. Open `FSD_Wizard.html` in a web browser (or visit the live link above)
2. Fill in your posting and family details
3. Click **Generate Entitlement Summary**
4. Review the summary cards and expand individual FSD sections for detail
5. Use the source links in the tool to verify the governing directive language

## Rates in use

| Table | Effective date |
|---|---|
| FSP, PDA, Posting Loan maximum | April 1, 2026 |
| Shelter Contribution (FSD 25, Appendix A) | April 1, 2026 |
| PSA, PLA | June 1, 2025 |

## Source basis

- [NJC Foreign Service Directives](https://www.njc-cnm.gc.ca/directive/fsd-dse/en)
- [FSD 25 Appendix A — Shelter Contribution Table](https://www.njc-cnm.gc.ca/directive/d114/v307/s919/en)

## Technical notes

Single-file application — `FSD_Wizard.html` — built with plain HTML, CSS, and JavaScript. No framework, no build step, no backend. The feedback form uses Formspree (`xojyjzvk`).

## Disclaimer

This is an independent hobby project. It is not affiliated with the Government of Canada or the NJC. Use it as a structured starting point, not as an official entitlement determination. Always confirm with your departmental FSD administrator and the NJC source text.

## Feedback

Use the feedback link inside the tool, or [open an issue](https://github.com/manojsarang/fsd-wizard/issues).

If it has been useful, [buying me a coffee](https://www.paypal.com/donate/?business=s.manojrao%40gmail.com&currency_code=CAD&item_name=FSD+Wizard) is appreciated.
