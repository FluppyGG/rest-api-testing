# Simulated Defect Examples

These examples are intentionally written as portfolio exercises. They do **not** claim real defects in JSONPlaceholder.

## API-001 - Duplicate payment command is processed twice

**Severity:** Critical  
**Type:** Idempotency / payment flow

**Scenario:** The same payment request is resent after a client timeout using the same idempotency key.

**Expected:** The server returns the original operation result and does not create a second payment.

**Observed in simulated system:** Two payment records are created.

**Evidence to attach in a real project:** request IDs, timestamps, payloads, idempotency key, transaction IDs, DB rows and backend logs.

## API-002 - Role-restricted entity is returned to read-only user

**Severity:** High  
**Type:** Authorization

**Expected:** 403 Forbidden.  
**Observed in simulated system:** 200 OK with full entity payload.
