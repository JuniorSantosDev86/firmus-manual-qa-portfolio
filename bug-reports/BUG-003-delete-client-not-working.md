# BUG-003 — Delete client action does not remove the client after confirmation

| Field | Information |
|---|---|
| Bug ID | BUG-003 |
| Module | Clients |
| Environment | Local development |
| Browser | Google Chrome |
| Operating System | Ubuntu Linux |
| Device / Viewport | Desktop |
| Severity | High |
| Priority | High |
| Status | Open |
| Reported by | Ademir dos Santos Junior |
| Reported date | 2026-04-24 |

---

## Summary

When the user clicks the delete client button and confirms the deletion in the popup, the client is not removed.

---

## Preconditions

- The application is running locally.
- The user is authenticated.
- The user is on the clients page.
- At least one client record exists.
- The delete client action is available.

---

## Steps to Reproduce

1. Open the Firmus application.
2. Log in with valid credentials.
3. Navigate to the clients area.
4. Select an existing client or locate the delete client action.
5. Click the delete client button.
6. Confirm the deletion in the popup.
7. Observe the client list after confirmation.

---

## Actual Result

The confirmation popup appears and the user confirms the deletion, but the client is not removed from the list.

---

## Expected Result

After confirming deletion, the selected client should be removed from the client list and the system should provide clear feedback that the deletion was completed.

---

## Evidence

- Screenshot: `../evidences/screenshots/BUG-003-delete-client-not-working.png`

Optional:

- Video: `../evidences/videos/BUG-003-delete-client-not-working.mp4`

---

## Additional Notes

This issue was found during exploratory observation while testing the Clients module. Although it was not part of the original detailed test cases, it affects client management and should be documented.