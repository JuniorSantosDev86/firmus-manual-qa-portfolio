# BUG-004 — Quote can be created with empty or invalid required fields

| Field | Information |
|---|---|
| Bug ID | BUG-004 |
| Module | Quotes |
| Environment | Local development |
| Browser | Google Chrome |
| Operating System | Ubuntu Linux |
| Device / Viewport | Desktop |
| Severity | Medium |
| Priority | Medium |
| Status | Open |
| Reported by | Ademir dos Santos Junior |
| Reported date | 2026-04-24 |

---

## Summary

The system allows a quote to be created with empty fields or invalid/random data in required fields.

---

## Preconditions

- The application is running locally.
- The user is authenticated.
- The user is on the quotes page.
- The quote creation flow is available.

---

## Steps to Reproduce

1. Open the Firmus application.
2. Log in with valid credentials.
3. Navigate to the quotes area.
4. Click the action to create a new quote.
5. Leave required fields empty or fill them with invalid/random data.
6. Submit the form.
7. Observe the system behavior.

---

## Actual Result

The quote is created successfully even when required fields are empty or contain invalid/random data.

---

## Expected Result

The system should prevent quote creation when required fields are empty or contain invalid data, and should display clear validation messages for the affected fields.

---

## Evidence

- Screenshot: `../evidences/screenshots/BUG-004-quote-created-with-empty-or-invalid-fields.png`

---

## Additional Notes

This issue may affect data quality because quote records can be created without reliable or valid business information.