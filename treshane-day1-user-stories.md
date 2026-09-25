# LearnLanka — User Story Set v0.1

## Story 1: Find a Tutor Who Teaches in My Language

As a student

I want to find tutors by subject, grade, language and price

So that I only see tutors I can understand and afford

### Acceptance Criteria

- Given I choose Maths, O/L, Sinhala and under Rs 2,000 when I search then I only see approved tutors who match all four
- Given no tutor matches my filters when I search then I see a message saying so and a suggestion to widen the price range
- Given I'm looking at the results when they load then each one shows the tutor's name, subjects, language, hourly price and rating

### INVEST Self Check

- [x] Independent
- [x] Negotiable
- [x] Valuable
- [x] Estimable
- [x] Small
- [x] Testable

## Story 2: Book and Pay for a Session

As a student

I want to book a free 1 hour slot and pay by card or eZ Cash

So that my place with the tutor is confirmed

### Acceptance Criteria

- Given a tutor has a free slot when I pay for it successfully then the booking goes to the tutor and the slot disappears for everyone else
- Given my payment fails when I return to the app then no booking is created and the slot is still free
- Given two students pick the same slot when both try to pay then only the first one gets the booking

### INVEST Self Check

- [ ] Independent: needs Story 4, because tutors have to publish slots first
- [x] Negotiable
- [x] Valuable
- [x] Estimable
- [ ] Small: booking and payment together might be too big for one sprint, so it may need splitting
- [x] Testable

## Story 3: Cancel a Booking and Get My Money Back

As a student

I want to cancel a booking I can no longer attend

So that I don't lose money if I give enough notice

### Acceptance Criteria

- Given my session is 12 or more hours away when I cancel then I get a full refund and the tutor is told
- Given my session is less than 12 hours away when I try to cancel then I'm warned that I won't get a refund before I confirm

### INVEST Self Check

- [ ] Independent: only works once Story 2 exists
- [ ] Negotiable: the 12 hour rule for students is our assumption and still needs the founders' approval
- [x] Valuable
- [x] Estimable
- [x] Small
- [x] Testable

## Story 4: Publish My Available Times

As a tutor

I want to publish the 1 hour slots I'm free for

So that students can book me when it suits me

### Acceptance Criteria

- Given I'm an approved tutor when I publish a slot then students can see it on my profile
- Given a slot hasn't been booked when I remove it then students can no longer see it
- Given a slot has already been booked when I try to remove it then I'm told to cancel the booking instead

### INVEST Self Check

- [x] Independent
- [x] Negotiable
- [x] Valuable
- [x] Estimable
- [x] Small
- [x] Testable

## Story 5: See What I Earned

As a tutor

I want to see the price, commission and my share for each completed session

So that I know exactly what I'll be paid and why

### Acceptance Criteria

- Given I completed a Rs 2,000 session when I open my earnings then I see Rs 2,000, Rs 300 commission and Rs 1,700 to me
- Given a session didn't count as completed when I open my earnings then it shows no commission and no payment

### INVEST Self Check

- [ ] Independent: it relies on the completed session rule, which the founders haven't confirmed
- [x] Negotiable
- [x] Valuable
- [x] Estimable
- [x] Small
- [x] Testable

## Story 6: Approve New Tutors

As an ops admin

I want to review each tutor application and approve or reject it

So that only checked tutors can teach students

### Acceptance Criteria

- Given a new application when I open it then I can see the tutor's ID and qualification documents in one place
- Given I reject an application when I save my decision with a reason then the tutor is told why and doesn't appear in search
- Given I approve an application when I save it then the tutor can start publishing slots

### INVEST Self Check

- [x] Independent
- [x] Negotiable
- [x] Valuable
- [ ] Estimable: the brief never says what vetted involves, so we can't size the checks yet
- [x] Small
- [x] Testable

## Story 7: Pay Tutors Every Week

As an ops admin

I want to run one weekly payout for every tutor

So that tutors are paid correctly without me checking each one by hand

### Acceptance Criteria

- Given it's Tuesday when I run the payout then I see each tutor's 85% share of last week's completed sessions
- Given the bank confirms a payment when I mark it as paid then the tutor sees it as paid in their earnings

### INVEST Self Check

- [ ] Independent: needs Story 5's earnings figures
- [x] Negotiable
- [x] Valuable
- [ ] Estimable: we don't know yet if the bank accepts an automatic file or needs a manual upload
- [ ] Small: probably two stories, working out the payout and then recording the bank's confirmation
- [x] Testable

## Story 8: Fast Search on Mobile Data

Non functional requirement

As a student on a phone with mobile data

I want search results to appear quickly

So that I don't give up or waste my data waiting

### Acceptance Criteria

- Given I'm on a Sri Lankan 4G connection when I search for tutors then results appear in under 800 ms for at least 95% of searches
- Given the target is missed in any hour when the team checks monitoring then an alert has already been raised

### INVEST Self Check

- [x] Independent
- [ ] Negotiable: the founders set the 800 ms target, so it's fixed
- [x] Valuable
- [x] Estimable
- [ ] Small: speed affects all of search, not just one feature
- [x] Testable