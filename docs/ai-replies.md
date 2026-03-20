# AI Replies – Passporta

All status messages are defined in `ai/statuses.json`.
This file documents the intent and communication goal for each status.

---

## unpaid
**Used when:** application has not been paid for yet.
**Goal:**
- inform the customer payment is required
- prompt action without being aggressive

---

## underpayment
**Used when:** payment received but amount is insufficient.
**Goal:**
- clearly flag the shortfall
- prompt the customer to complete payment

---

## status-0 — Waiting to assign
**Used when:** application received but not yet assigned to a team member.
**Goal:**
- reassure customer their application was received
- set expectation that processing hasn't started yet

---

## status-1 — Processing
**Used when:** application is actively being worked on.
**Goal:**
- reassure customer
- avoid giving exact timeframes
- confirm application is active

(see `ai/templates/status_processing.txt`)

---

## status-2 — Approved
**Used when:** e-visa has been approved.
**Goal:**
- deliver good news clearly
- inform customer to check email for the visa

---

## status-3 — To refund
**Used when:** refund has been initiated but not yet processed.
**Goal:**
- confirm refund is in progress
- set expectation of up to 5 business days

---

## status-4 — Refunded
**Used when:** refund has been completed.
**Goal:**
- confirm refund was sent
- reference original payment method

---

## status-5 — Incomplete
**Used when:** application is missing required information.
**Goal:**
- alert the customer clearly
- direct them to check email for specific instructions

---

## status-6 — Pending
**Used when:** application is queued for review.
**Goal:**
- reassure customer it's in the queue
- avoid implying any problem

---

## status-7 — On hold
**Used when:** application has been paused for any reason.
**Goal:**
- be transparent that progress is paused
- direct customer to email or support

---

## status-8 — Missing documents
**Used when:** specific documents are still needed.
**Goal:**
- clearly flag the issue
- direct customer to email for details

---

## status-9 — Cancelled
**Used when:** application has been cancelled.
**Goal:**
- communicate clearly and neutrally
- avoid alarming language

---

## status-10 — Refused
**Used when:** immigration authorities have refused the application.
**Goal:**
- deliver difficult news professionally
- attribute decision to authorities, not Passporta

---

## status-11 — Via agent
**Used when:** application is being handled by an external agent.
**Goal:**
- reassure customer their case is being handled
- no need to contact main support

---

## status-12 — Pending payment
**Used when:** payment step is not yet completed.
**Goal:**
- prompt customer to complete payment
- do not suggest application is lost or cancelled

---

## status-13 — Delayed
**Used when:** processing is taking longer than usual.
**Goal:**
- acknowledge the delay honestly
- apologize without over-promising

---

## status-14 — Sensitive Data Deletion
**Used when:** GDPR/data deletion request is being processed.
**Goal:**
- confirm the request is being handled
- reassure customer data is being treated securely

---

## status-15 — Travel Date Passed
**Used when:** the customer's travel date is in the past.
**Goal:**
- acknowledge the situation
- direct to support for next steps
