# Restful-Booker API — Manual Test Cases

**API Base URL:** https://restful-booker.herokuapp.com
**Tool Used:** Postman
**Documentation:** https://restful-booker.herokuapp.com/apidoc/index.html

## 1. Health Check & Read (GET)

| ID | Title | Method | Endpoint | Expected Status | Expected Result |
|---|---|---|---|---|---|
| API-GET-001 | Verify API is online | GET | `/ping` | 201 | Returns "Created" (Health check) |
| API-GET-002 | Get all booking IDs | GET | `/booking` | 200 | Returns an array of JSON objects with `bookingid` |
| API-GET-003 | Get specific booking by ID | GET | `/booking/1` | 200 | Returns full booking details (First name, Last name, etc.) |
| API-GET-004 | Get booking with invalid ID | GET | `/booking/999999` | 404 | Returns "Not Found" |

## 2. Create (POST)

| ID | Title | Method | Endpoint | Expected Status | Expected Result |
|---|---|---|---|---|---|
| API-POST-001 | Create a new booking | POST | `/booking` | 200 | Returns a new `bookingid` and booking details |
