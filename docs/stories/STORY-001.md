# STORY-001: Health endpoint
Ticket: [ZOU-9](/ZOU/issues/ZOU-9) · Size: S (one day or less) · Data class: INTERNAL

## Why
The agency needs the smallest possible app to prove the Developer 1 → QA → Tech Lead → Board pipeline works.

## Acceptance criteria
- Given the app is running, When I send `GET /health`, Then I get HTTP 200 and the JSON body `{"ok": true}`.
- Given the repo, When I run `make check`, Then it passes lint, types, and tests.
- Given the repo, When I read `README.md`, Then it says how to run the app and the tests.

## Files likely to touch
- `app/main.py`
- `tests/test_health.py`
- `pyproject.toml`
- `uv.lock`
- `README.md`

## Out of scope
- Database access
- Authentication
- AI features

## Test notes (edge cases QA must try)
- Confirm the response body is exactly `{"ok": true}`.
- Confirm the documented server port is 8001, not the local model port 8000.
