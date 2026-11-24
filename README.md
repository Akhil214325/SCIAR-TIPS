
# Sciar Tips – CA2 Submission

**GitHub Pages:** https://akhil214325.github.io/SCIAR-TIPS/

**GitHub Repository:** https://github.com/akhil214325/SCIAR-TIPS

## Product question

How can a staff-facing tip view make the payout calculation more understandable and give a less powerful employee a visible route to raise a concern without exposing colleagues' individual data?

## Part 1: The People

**Internal – Aoife Rennick (CEO, Sciar):** “Make it work on a phone. Nearly all restaurant staff only have phones.” (04-aoife.md). Her need: a staff view that works on a phone before Friday's investor meeting.

**External – Rafael (kitchen porter, Halloran's):** “i dont understand how they count it.” and “please dont say it was me who ask” (01-rafael.md). His need: to see how his payout is calculated, and to question it without being named.

**Cultural difference and accessibility:** Rafael's first language is Portuguese and his phone screen is broken (01-rafael.md), so app.html uses large figures, short plain-English sentences and a one-line Portuguese summary.

## Part 4a: Theory Behind the Build

**Leadership – paternalistic leadership (Pellegrini & Scandura, 2008).** Declan sets the rule alone (“I've been in this trade 22 years”) and helps staff personally (Rafael's visa letter). This explains Rafael's loyalty and fear: “i dont want problem with Declan”. It misses the system: the rule, not Declan's kindness, decides that Rafael's after-23:00 hours earn nothing.

**Culture – organisational silence (Morrison & Milliken, 2000).** Niamh says “Nobody has ever complained about the split. Not once in twelve weeks.” (03-niamh.md), but Rafael asked her and was told “is the system, is fair for everybody”. Silence is not agreement.

**Design choice:** because of silence, concerns go to Sciar, not the owner or floor manager, and the page shows what Rafael cannot see: 34% of his hours earned no points.

**Competitive advantage:** staff trust in the numbers is harder to copy than a payment pipe.

**Limit:** neither theory says whether the rule is fair, only why nobody questions it.

**References**

- Morrison, E. W. and Milliken, F. J. (2000). Organizational silence: A barrier to change and development in a pluralistic world. *Academy of Management Review*, 25(4), 706–725.
- Pellegrini, E. K. and Scandura, T. A. (2008). Paternalistic leadership: A review and agenda for future research. *Journal of Management*, 34(3), 566–593.

## Part 4b: Decision Record

**Decision 1 – Request refused: Niamh and Aoife asked me to remove the concern feature** (03-niamh.md; 04-aoife.md, point 3). Options: remove it; send concerns to owner and floor manager; send them to Sciar only. Criteria: a voice for the least powerful user, Rafael's privacy, owners not feeling attacked. Deciding factor: Rafael already went to Niamh and it did not help. I kept it, Sciar-only and simulated in the browser (stated on the page). Underlying need: there is no public “moaning wall”, and Sciar checks figures before raising anything with the owner. Would change my mind: evidence of a safe, independent route staff already use.

I also left out Declan's “100% of tips go to the team” and “Fully compliant with Irish tips law” (02-declan.md): card tips reach staff, but the €9,004.69 service charge goes to the house (takings.csv, service_charge_paid_to = house), so readers could misread it, and legal claims are not allowed.

Decision 2 – AI market-scan suggestion

I considered using the AI-generated 34% retention figure and the claim that Sciar was “only fully compliant”, but rejected both because no reliable sources supported them. A verifiable study and independent evidence could change my decision.

Bias: I noticed automation bias when I initially trusted the precise 34% figure because it sounded authoritative, before checking its evidence.

## Part 4c: The Struggle

I created a website for Sciar Tips. It has a landing page for the business and a dashboard for staff. The project was not always easy. At first the dashboard did not display correctly, and an unwanted prototype warning kept appearing. I fixed these problems by correcting the HTML code and updating the files on GitHub. I used AI to help me understand the code and find ways to improve it. However, I did not just copy its suggestions. I checked them myself and tested them before using them. Through this work, I learned a lot about building websites and presenting data clearly. I also thought about employee privacy and why it is important to be open with staff about their data. If I did this project again, I would test it more carefully, improve the security, and make it more accessible on mobile phones.

<img width="1481" height="838" alt="4" src="https://github.com/user-attachments/assets/2092c603-a681-478d-a55d-85636efdc5fb" />
<img width="1467" height="882" alt="3" src="https://github.com/user-attachments/assets/dc649940-d2df-4820-8d2d-6b45067273b4" />
<img width="1728" height="797" alt="2" src="https://github.com/user-attachments/assets/fd2bb3c1-b14f-4f79-aac0-80ef779f33f0" />
<img width="1857" height="797" alt="1" src="https://github.com/user-attachments/assets/1475af54-b812-488e-9f9e-13aa5af27f56" />



