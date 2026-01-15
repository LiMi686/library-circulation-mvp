# Data Dictionary (Synthetic) — Main Library Circulation

## items
- item_id: string, unique
- collection: category {Book, DVD, Laptop, CourseReserve}
- subject: category {HSS, STEM, Law, Business, Medicine, Arts}
- loan_policy_days: int (e.g., 1, 3, 7, 14, 28)
- home_location: constant "Main"

## patrons (anonymized)
- patron_id: string, unique
- patron_group: category {Undergrad, Grad, Faculty, Staff, Community}
- risk_profile: category {low, medium, high}  (late-return tendency)

## circulation_transactions
- txn_id: string, unique
- checkout_dt: datetime
- due_dt: datetime
- return_dt: datetime or null (not returned yet)
- renewal_count: int >= 0
- item_id: fk -> items.item_id
- patron_id: fk -> patrons.patron_id
- checkout_location: constant "Main"

## holds
- hold_id: string, unique
- request_dt: datetime
- fulfill_dt: datetime or null
- status: category {fulfilled, cancelled, expired, pending}
- item_id: fk -> items.item_id
- patron_id: fk -> patrons.patron_id
- pickup_location: constant "Main"

## Privacy Note
All data is synthetic and contains no PII. Distributions are simulated to resemble academic library circulation patterns.
