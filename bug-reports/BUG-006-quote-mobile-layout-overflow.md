# BUG-006 — Quote layout breaks on mobile-like viewport

| Field | Information |
|---|---|
| Bug ID | BUG-006 |
| Module | Quotes |
| Environment | Local development |
| Browser | Google Chrome |
| Operating System | Ubuntu Linux |
| Device / Viewport | Mobile-like viewport |
| Severity | Medium |
| Priority | Medium |
| Status | Open |
| Reported by | Ademir dos Santos Junior |
| Reported date | 2026-04-24 |

---

## Summary

The quotes page has a responsive layout issue where a box overflows or breaks the layout on a mobile-like viewport.

---

## Preconditions

- The application is running locally.
- The user is authenticated.
- The user is on the quotes page.
- The page is being tested using a mobile-like viewport.

---

## Steps to Reproduce

1. Open the Firmus application.
2. Log in with valid credentials.
3. Navigate to the quotes area.
4. Enable a mobile-like viewport using browser DevTools or resize the browser window to a mobile width.
5. Observe the quotes page layout.
6. Check whether all boxes and content fit correctly within the viewport.

---

## Actual Result

A box overflows or breaks the layout in the mobile-like viewport.

---

## Expected Result

The quotes page should adapt correctly to the mobile-like viewport, keeping all boxes and content readable, aligned and contained within the screen width.

---

## Evidence

- Screenshot: `../evidences/screenshots/BUG-006-quote-mobile-layout-overflow.png`

---

## Additional Notes

This issue affects responsive usability and may reduce the quality of the experience for users accessing the application from smaller screens.