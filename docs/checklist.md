# REST API QA Checklist

## Request
- Correct method and URL
- Required path/query parameters
- Required headers
- Correct Content-Type
- Valid and invalid payloads

## Response
- Status code
- Response headers
- JSON parseability
- Required fields
- Field types
- Field values / constraints
- Error object quality
- Response time sanity

## Cross-checks for a real product
- UI vs API state
- API vs database state
- role / permission behavior
- retry and idempotency behavior
- duplicate request handling
- audit log creation
