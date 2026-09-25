LearnLanka — Ambiguity Hunt Log

 connects O/L and A/L students, vetted tutors, price band, pay via card or eZ Cash, cancel with at least 12 hours notice, 15% commission on every completed session, pay tutors weekly via bank transfer, Mobile first … 80% Android, 200 simultaneous video sessions, under 800 ms … from a Sri Lankan ISP, 99.5% monthly uptime, measured against the booking endpoint, three contradictory expectations from the founders

## Findings

| # | Quote | Why ambiguous | Clarification question | Priority |
|---|---|---|---|---|
| 1 | cancel with at least 12 hours notice | The rule is only written for tutors. It says nothing about students cancelling or who gets refunded. | If a student cancels less than 12 hours before, do they get a full, partial or no refund? Is there a penalty for a tutor who cancels late? | H |
| 2 | 15% commission on every completed session | Completed isn't defined. A call could drop, end early, or one person might not show up. | Does a session count as completed if it lasts under 60 minutes? If the student doesn't join, is the tutor still paid? | H |
| 3 | connects O/L and A/L students | Most of these students are under 18, and Sri Lanka's data protection law has extra rules for children. Parents aren't mentioned. | Do students under 18 sign up themselves, or must a parent or guardian create the account and give consent? | H |
| 4 | vetted tutors | It doesn't say who checks tutors or what they check. | What must a tutor provide before approval: ID, certificates, a police report, a demo class? Who approves them? | M |
| 5 | pay via card or eZ Cash | It doesn't say when the money is taken or if the gateway supports both methods. | Is the student charged when booking or after the session? Does our payment gateway accept eZ Cash? | H |
| 6 | Mobile first … 80% Android | This could mean a Play Store app or a website that works well on phones. | Are we building a native Android app, or a mobile website? Is iPhone support needed at launch? | H |
| 7 | price band | It doesn't say who sets the bands or how many there are. | Does LearnLanka set fixed bands, or can tutors choose any price? What are the band limits in rupees? | L |
| 8 | 200 simultaneous video sessions | This could mean 200 calls (400 people) or 200 people. Video is charged per minute, so the cost doubles. | Does 200 mean 200 calls or 200 participants at the same time? | M |
| 9 | pay tutors weekly via bank transfer | No payout day, minimum amount or fee owner is given. | Which day are tutors paid? Is there a minimum payout? Who pays the transfer fee? | M |
| 10 | under 800 ms … from a Sri Lankan ISP | It doesn't say which ISP, which connection type or where it's measured. | Is 800 ms measured on a phone using mobile data, or at our server? Which ISP do we test from? | M |
| 11 | 99.5% monthly uptime, measured against the booking endpoint | If video is down but booking works, it's unclear whether the app counts as up. | Does a video outage count against the 99.5% target, or only booking failures? | M |
| 12 | three contradictory expectations from the founders | The brief mentions them but never says what they are. | What are the three expectations, and which founder owns each decision? | H |

## Results Summary

| Metric | Target | Achieved |
|---|---|---|
| Items found | 10+ | 12 |
| High priority items | 3+ | 6 |
| Items convertible to test cases | 5+ | 7 (rows 1, 2, 5, 8, 9, 10, 11) |

## Top 3 Questions to Ask the Founders

1. What are your three conflicting expectations, and who decides each one?

2. Are we building a native Android app or a mobile website?

3. Do students under 18 need a parent or guardian to create their account and give consent?

