# REST API Testing Portfolio

A compact Manual QA portfolio project demonstrating REST API testing with Postman/Newman.

## What this repository demonstrates

- positive and negative API checks;
- validation of HTTP status codes, headers and JSON payloads;
- request/response consistency checks;
- basic data validation across related endpoints;
- reusable Postman environment variables;
- CLI execution with Newman;
- CI execution in GitHub Actions;
- concise test planning and defect documentation.

The public JSONPlaceholder API is used as a safe training target. The repository is a **QA lab / portfolio project**, not a claim of production defects in that service.

## Quick start

```bash
npm install
npm test
```

Or run directly:

```bash
npx newman run postman/jsonplaceholder-qa.postman_collection.json \
  -e postman/local.postman_environment.json
```

## Coverage

| Area | Examples |
|---|---|
| GET | entity retrieval, filtering, 404 path |
| POST | payload acceptance and response validation |
| PUT | full update response checks |
| Data | required fields, types, cross-field checks |
| Negative | non-existing resource, invalid assumptions |
| CI | automated Newman run on push / pull request |

## Portfolio talking points

1. Explain why status-code-only checks are insufficient.
2. Show how response body assertions catch contract regressions.
3. Explain the difference between API functional checks and persistence checks.
4. Discuss what would be added for authentication, rate limits, idempotency and contract testing in a real product.
