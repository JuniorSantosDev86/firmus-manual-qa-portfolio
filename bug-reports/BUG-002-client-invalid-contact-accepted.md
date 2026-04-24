# BUG-002 — Client can be created without valid contact information

| Field | Information |
|---|---|
| Bug ID | BUG-002 |
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

The system allows a client to be created without contact information or with invalid contact information.

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
5. Fill the required visible fields.
6. Leave contact information empty or enter invalid contact information.
7. Submit the form.
8. Observe the system behavior.

---

## Actual Result

The client is created successfully without valid contact information.

---

## Expected Result

The system should either require valid contact information or display a clear validation message when contact information is missing or invalid.

---

## Evidence

- Screenshot: `../evidences/screenshots/BUG-002-client-invalid-contact-accepted.png`

---

## Additional Notes

This issue may affect client communication and downstream operational workflows.