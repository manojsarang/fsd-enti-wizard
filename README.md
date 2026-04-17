# fsd-enti-wizard
# FSD Wizard

FSD Wizard is a personal browser-based reference tool for understanding potential Canadian Foreign Service entitlements under the National Joint Council Foreign Service Directives.

It helps a user turn a posting profile into a structured summary of likely allowances, travel-related provisions, and key administrative requirements. It is designed as a practical reference tool, not an official entitlement decision system.

## Overview

The tool is intended to help Foreign Service employees and families answer questions such as:

- What allowances may apply at this post?
- What changes based on hardship level, dependants, or tour length?
- What should I expect to review with an FSD Administrator?
- Which FSD sections are relevant to my situation?

The goal is to provide a clearer starting point before or during a posting abroad.

## Features

- Browser-based calculator with no installation required
- Single profile form covering employment, family, posting, housing, vehicle, and daycare inputs
- Estimated annual allowance summary where rate-based calculations are possible
- Expandable results by FSD section
- Embedded explanations for key entitlements and conditions
- Searchable post selector with auto-fill for hardship level and unhealthy post status
- Direct links back to the NJC Foreign Service Directives
- Feedback form for bugs, suggestions, and general comments

## Covered Areas

The tool includes guidance or calculations related to topics such as:

- Posting Loan
- Relocation
- Principal Residence
- Spouse or common-law partner assistance
- Special Family Separation Assistance
- Shelter
- Transportation at post
- Daycare
- Education and education travel
- Preventive medical and health-related provisions
- Post Travel Assistance
- Family Reunion Travel
- Compassionate Travel
- Post Living Allowance
- Foreign Service Premium
- Post Specific Allowance
- Post Differential Allowance
- Emergency evacuation and loss
- Allowance reporting and certification requirements

## How to Use

1. Open `FSD_Wizard.html` in a web browser.
2. Enter the relevant profile details.
3. Click **Calculate My Entitlements**.
4. Review the summary cards and expand individual FSD sections for detail.
5. Use the source links in the tool to verify the governing directive language.

## Source Basis

The tool is based primarily on:

- NJC Foreign Service Directives, April 1, 2025 edition
- NJC Guide to Rates and Allowances

The current implementation also embeds specific rate tables and post data directly in the HTML file.

According to the tool content, key rates currently reflected include:

- April 1, 2026 rates for FSP and PDA
- June 1, 2025 rates for PSA and PLA-related tables

These values should be reviewed periodically against current NJC sources.

## Important Notes

- This is a personal project.
- It is not affiliated with the Government of Canada or the NJC.
- It is a reference and decision-support tool only.
- It does not provide official entitlement determinations.
- Some entitlements are estimated or simplified for usability.
- Users should confirm final interpretations and payments with their departmental FSD Administrator.

## Privacy

The calculator logic runs in the browser.

Based on the current implementation:

- Profile data entered for calculations is not stored by the tool
- Profile data is not transmitted as part of the calculator workflow
- The site does not use cookies or tracking technologies

The only external submission in the current version is the feedback form.

## Feedback

The tool includes a feedback modal that collects:

- Name
- Email address
- Feedback type
- Message

Feedback is submitted through Formspree and is intended only to support follow-up on user feedback.

## Technical Notes

This project is intentionally simple.

- Single-file application: `FSD_Wizard.html`
- Built with plain HTML, CSS, and JavaScript
- No framework
- No build step
- No package manager
- No backend required for calculator functionality
- Formspree used only for feedback submission

The file contains:

- UI markup
- Styling
- Post and rate tables
- Input helpers
- Calculation logic
- Results rendering
- Feedback modal logic

## Project Structure

Current structure:

```text
.
└── FSD_Wizard.html
```

Everything is self-contained inside that file.

## Calculation Approach

The tool uses a combination of:

- Embedded rate lookups
- Rule-based conditional logic
- Post-specific mappings
- Explanatory sections for provisions that are not directly calculable

Examples include:

- FSP based on foreign service points and dependant count
- PDA based on hardship level and dependant count
- PSA based on selected post
- PLA based on salary band and post index
- Daycare estimates using embedded ceilings and employee share assumptions
- Education-related estimates based on child age categories

## Maintenance

Since this is a personal single-file project, the main maintenance tasks are straightforward:

- Update annual rates
- Update post-specific PSA data
- Update hardship and post condition data where needed
- Review explanatory text against current FSD wording
- Check external source links
- Confirm the feedback endpoint still works

## Configuration

The feedback form is configured in JavaScript using a Formspree form ID.

Current value in the file:

```js
const FORMSPREE_ID = 'xojyjzvk';
```

If feedback routing changes, that value needs to be updated.

## Possible Future Improvements

Potential future improvements could include:

- Adding a visible version number and last updated date
- Adding a changelog for rate updates
- Improving print output
- Adding export support for summaries
- Moving rate tables into separate data files for easier annual updates
- Tightening validation and input guidance for estimated fields

## Disclaimer

FSD Wizard is a personal reference project intended to help users understand possible Foreign Service entitlements and prepare better questions for official advisors. It should not be treated as an official interpretation of the Foreign Service Directives or as a substitute for departmental review.
