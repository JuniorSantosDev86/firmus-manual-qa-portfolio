# BUG-001 — Client can be created with only the name field filled

| Field | Information |
|---|---|
| Bug ID | BUG-001 |
| Module | Clients |
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

The system allows a client to be created with only the client name filled, without requiring additional client information.

---

## Preconditions

- The application is running locally.
- The user is authenticated.
- The user is on the clients page.
- The client creation flow is available.

---

## Steps to Reproduce

1. Open the Firmus application.
2. Log in with valid credentials.
3. Navigate to the clients area.
4. Click the action to create a new client.
5. Fill only the client name field.
6. Leave the remaining fields empty.
7. Submit the form.
8. Observe the system behavior.

---

## Actual Result

The client is created successfully even when only the name field is filled.

---

## Expected Result

The system should prevent incomplete client creation if additional fields are required, and should display clear validation messages for missing required information.

---

## Evidence

- Screenshot: `../evidences/screenshots/BUG-001-client-created-with-only-name.png`

---

## Additional Notes

This issue may affect data quality because client records can be created without enough information for future operational workflows.