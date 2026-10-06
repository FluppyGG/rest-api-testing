# API Test Plan

## Objective
Verify core behavior of a public REST API and demonstrate a repeatable QA approach.

## In scope
- response codes;
- JSON structure and required fields;
- filtering behavior;
- create/update response semantics;
- non-existing resources;
- basic response-time sanity checks.

## Out of scope
- load and stress testing;
- security penetration testing;
- real persistence guarantees of JSONPlaceholder;
- production SLA validation.

## Test design
- equivalence classes for valid / invalid identifiers;
- boundary-oriented checks around missing/non-existing resources;
- positive and negative scenarios;
- consistency checks for fields returned after create/update operations.

## Exit criteria
- all Newman checks pass;
- failed checks provide a clear assertion message;
- test data does not depend on local machine state.
