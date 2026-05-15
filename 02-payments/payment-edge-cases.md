## Transaction Consistency Risks

- Payment succeeds at bank but fails in application layer
- Duplicate charge due to retry after timeout
- Partial capture failure in multi-step payment flow

---

## Gateway & Third Party Failures

- Payment gateway returns success but webhook fails
- Gateway timeout after funds are reserved
- Inconsistent status between PSP and internal ledger

---

## Currency & Financial Accuracy

- Currency conversion mismatch between systems
- Rounding errors in multi-currency transactions
- Incorrect FX rate applied during transaction processing

---

## Retry & Concurrency Issues

- User clicks "Pay" multiple times
- Network retry causes duplicate transaction
- Race condition in payment confirmation callback
