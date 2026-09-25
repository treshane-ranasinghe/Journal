LearnLanka Requirements Document

1. Problem Statement

most O/L and A/L students find tutors through friends or Facebook ads. There's no easy way to compare tutors by subject, language and parents often pay upfront only to lose that money when a tutor cancels. Tutors have the opposite problem. They can't reach students outside their own town, and getting paid on time is a constant struggle. LearnLanka fixes this by letting students find a checked tutor who teaches in their language, book a one-hour online session and pay safely, while tutors get a steady stream of students and are paid every week.

2. Personas

(Student).A 16 year old and sitting her O/Ls in Kurunegala. She wants a Maths tutor who teaches in Sinhala, costs less than Rs 2,000 an hour and is free in the evenings. She's fed up with tutor ads that have no real reviews, and her family once lost money when a tutor cancelled on the day. Most learning apps she's tried are only in English.

(Tutor). A 27-year-old Physics teacher in Kandy who teaches in Tamil and English. He'd like to fill around 10 evening slots a week and have his pay arrive every week without chasing anyone. What bothers him most is students cancelling at the last minute and parents who pay late.

 (Operations Admin) works at LearnLanka's Colombo office. Her aim is to approve new tutors within 2 working days, sort out refund complaints quickly and make sure every tutor is paid correctly. At the moment, tutor documents are scattered across her inbox and she checks payouts by hand.

3. Functional Requirements

Student
1. Students can search for tutors by subject, grade, language Sinhala, Tamil or English and price band.
2. Every search result shows a card the tutor's name, subjects, language, hourly price and rating.
3. Students can book any available 1-hour slot.
4. Students can pay by card or eZ Cash, and the tutor only sees the booking once payment has gone through.
5. Students who cancel at least 12 hours before the session get their money back in full.
6. After a completed session, students can give the tutor 1 to 5 stars and a one-line comment.
7. Students can ask for their account and personal data to be deleted.

Tutor

8. Tutors can publish the 1-hour slots they're available for.
9. Tutors can accept or decline each booking.
10. Tutors can only cancel if the session is at least 12 hours away, and the student is refunded in full.
11. After a completed session, tutors can give the student 1 to 5 stars and a one-line comment.
12. Tutors can see what each completed session cost, the 15% commission taken and how much they'll receive.

Operations Admin

13. Admins can approve or reject tutor applications. Tutors who haven't been approved don't show up in search.
14. Admins can give a full or partial refund when a session is disputed.
15. Admins can run the weekly payout, which sends each tutor 85% of their completed sessions by bank transfer.
16. Admins can view data deletion requests and mark them as done.

4. Non-Functional Requirements

1. Speed: 95% of tutor searches return results in under 800 ms. We'll measure this with Azure Application Insights, tested from a Sri Lankan 4G connection.
2. Availability: The booking endpoint is up 99.5% of the time each month. Azure Monitor will check it every minute.
3. Capacity: At least 200 video sessions can run at the same time. We'll check this on the video provider's dashboard and with a load test before launch.
4. Language: 100% of the app's text is available in Sinhala, Tamil and English. An automatic check for missing translations runs before every release.
5. Privacy:100% of accounts have recorded consent. A weekly database report should show 0 accounts missing it.
6. Payment security: LearnLanka stores no card details at all. Every payment is handled by PayHere.
7. Payouts: 100% of tutors are paid by Tuesday for the previous week. We'll check the payout report against the bank's confirmation.
