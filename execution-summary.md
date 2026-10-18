# API Test Execution Summary — Restful-Booker

**Execution Date:** October 2026
**Tool Used:** Postman
**Environment:** Production (Demo)
**Total Endpoints Tested:** 5

## Results
| Test ID | Endpoint | Method | Expected Code | Actual Code | Result |
|---|---|---|---|---|---|
| API-GET-001 | /ping | GET | 201 | 201 | PASS |
| API-GET-002 | /booking | GET | 200 | 200 | PASS |
| API-GET-003 | /booking/1 | GET | 200 | 200 | PASS |
| API-GET-004 | /booking/999999 | GET | 404 | 404 | PASS |
| API-POST-001 | /booking | POST | 200 | 200 | PASS |

## Evidence
- `GET-ping.png` — Health check returning 201 Created.
- `GET-all-bookings.png` — List of booking IDs.
- `GET-booking-1.png` — Specific booking details.
- `POST-create-booking.png` — New booking created (ID: 3053).
