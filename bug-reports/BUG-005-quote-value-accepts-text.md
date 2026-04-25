# BUG-005 — Quote value field accepts text instead of numeric value

| Field | Information |
|---|---|
| Bug ID | BUG-005 |
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

The system allows a quote to be created when the monetary value field is filled with text instead of a numeric value.

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
5. Fill the quote value field with text instead of a numeric value.
6. Fill the remaining fields as needed.
7. Submit the form.
8. Observe the system behavior.

---

## Actual Result

The quote is created successfully even when the monetary value field contains text instead of a numeric value.

---

## Expected Result

The system should reject text input in the monetary value field and display a clear validation message requiring a valid numeric value.

---

## Evidence

- Screenshot: `../evidences/screenshots/BUG-005-quote-value-accepts-text.png`

---

## Additional Notes

This issue may affect financial data quality because invalid monetary values can be saved in quote records.