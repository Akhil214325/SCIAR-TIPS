# Sciar Tips · CA2 submission

> Fictional teaching case for NCI. Sciar, Halloran's, their people and all case figures are invented.

## Links

- GitHub Pages: `https://YOUR-USERNAME.github.io/YOUR-REPOSITORY/`
- Repository: `https://github.com/YOUR-USERNAME/YOUR-REPOSITORY`

## Product question

How can a staff-facing tip view make the payout calculation more understandable and give a less powerful employee a visible route to raise a concern without exposing colleagues' individual data?

## Part 1: The people

Internal stakeholder – Aoife Rennick (CEO): “Make it work on a phone. Nearly all restaurant staff only have phones.” (04-aoife.md). External stakeholder – Rafael (kitchen porter): “i dont understand how they count it.” (01-rafael.md). Accessibility: Rafael’s first language is Portuguese and his phone screen is broken; the build uses a simple, mobile-first layout with clear figures and plain language. His concern is saved visibly on his device, with storage limits disclosed.

## Part 2: The build

The staff page is `app.html`. It uses the supplied `data/payouts.js`, which contains the same 152 observed rows as `data/payouts.csv`. The example profile is Rafael, a kitchen porter. Across weeks 1–12, the data records €679.02 in payouts, 527.5 hours worked and 178.5 hours after 23:00. The current rule gives no points for those late hours; Rafael's points total 87.24.

The additional group figure is tips per eligible hour, calculated as sum of `tip_payout_eur` divided by sum of (`hours` − `hours_after_2300`) for weeks 1–12. The page suppresses roles with fewer than three distinct staff IDs. In this dataset it displays servers (5 people; €7.78 per eligible hour) and chefs (3 people; €3.89 per eligible hour). Source and filter are shown on screen. These are group averages, not a claim that roles or individuals are directly comparable.

The concern form stores the text in browser local storage on the same device. It is a simulation, not a secure or transmitted complaint channel. The prototype profile is fixed to Rafael and is not an authenticated production account.

## Part 3: The landing page

`index.html` is a separate page for restaurant owners. It makes three pack-supported statements: weekly Monday payout process, the twelve-week Halloran's teaching-case pilot, and the staff-only view of individual payouts. Each statement names its source in the page. The call to action is an illustrative `mailto:hello@sciar.example` address; it is not monitored. No unsupported market, testimonial, rating, legal or regulatory claims are used.

## Part 4a: Theory behind the build

A transformational leadership lens (Bass, 1985) helps explain Aoife’s push for a phone-first alpha before investor meetings: she sets a clear direction and mobilises the small team around a visible product deadline. It does not explain whether that direction gives less powerful staff meaningful voice; investor urgency can crowd out challenge. Schein’s culture model (2010) distinguishes visible artefacts, espoused values and underlying assumptions. The staff text and owner-controlled points rule are artefacts; Declan’s statement that staff “don't need the formula” signals an assumption that transparency creates conflict. Rafael’s message challenges that assumption. The dashboard therefore shows the points rule and a concern-record feature while suppressing individual colleague data. A psychologically safer route to raise concerns can help Sciar differentiate through trust and retention of restaurant relationships, but these theories cannot establish that the product will cause better retention or prove the rule is fair. References: Bass (1985), *Leadership and Performance Beyond Expectations*; Schein (2010), *Organizational Culture and Leadership* (4th ed.).

## Part 4b: Decision record

**Decision 1 – Declan’s landing-page request.** Options: publish “Fully compliant with Irish tips law” and “100% of tips go to the team”, or omit those claims. Criteria: truth, evidence and risk of misleading owners. The pack contains no legal analysis, and the observed payout total is €31,754.09 against a €31,754.13 card-tip pool (rounding difference €0.04); therefore I would omit both absolute claims. The page instead describes the weekly process without a compliance promise. Evidence that the legal claim is verified or a reconciled accounting treatment would change this decision.

**Decision 2 – AI market-scan recommendation.** Options: use or reject the 34% retention and “only fully compliant” claims. I reject them because no sources were attached and the case instructions prohibit unsupported claims. A verifiable primary study and independent legal review would change my view.

**Bias to check:** confirmation/automation bias – I was initially drawn to the AI’s precise 34% figure because it sounded authoritative, before checking that it had no supporting source. These are proposed decisions; confirm that they match the choices you actually made.

## Part 4c: The Struggle (write this yourself – no AI)

**Do not submit AI-generated text here.** Write 100–150 words in your own voice. Describe what you tried, what broke, one AI output you personally checked or corrected, what you would do differently, and include an actual commit hash from your repository. Do not invent a commit hash.

## Part 5: Published

Repository checklist:
- [ ] Public GitHub repository contains `index.html`, `app.html`, `README.md`, `data/payouts.csv`, `data/takings.csv`, `data/payouts.js`, `data/takings.js` and `ai-log/`.
- [ ] GitHub Pages is enabled and serves the repository.
- [ ] Both pages work from the live URL in a private/incognito window.
- [ ] AI session evidence is saved in `ai-log/` (exports, share links or screenshots). Add your real session evidence; do not treat this generated README as a substitute.
- [ ] Replace both placeholder GitHub links above.
- [ ] Export this README as PDF and submit that single PDF through Moodle Turnitin by the deadline.

## Assumptions and limitations

- The fixed Rafael profile is a demonstration, not a secure multi-user login.
- The concern log is local to the browser and is not transmitted to Sciar, Halloran's or an independent recipient.
- The group comparison uses eligible hours (hours less hours after 23:00) as the denominator. Only groups of at least three distinct staff are shown.
- The pack's observed data and message claims are kept distinct. The AI market scan is treated as an unsupported claim, not as verified market evidence.
- The assessment case is set in 2028; all entities and numbers are fictional.
