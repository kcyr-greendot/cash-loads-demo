# Claude Guidelines — cash-loads-demo

## Project Overview

A standalone, single-file (`index.html`) browser-based demo of the **Green Dot Network Cash Loads** solution. No server or internet connection required.

**What it is:** A desktop browser page containing a mobile-device frame that simulates a partner's app walking through the cash load flow. Alongside the simulated app, the page shows screen-specific commentary, details, and documentation links for the sales rep to reference during a demo.

**Base brand:** "Chirp" (Green Dot's internal mock brand). Partner theming can be applied by overriding CSS variables and swapping a logo — no code changes needed.

**Simulated flow:**
1. Access the cash loads option within the partner app
2. Select a retail location
3. Generate a barcode
4. Simulate scanning the barcode at a retailer
5. Simulate cash remittance
6. Record and confirm the load

**Architecture constraints:**
- Single HTML file — all CSS and JS inlined or bundled; no external network calls at runtime
- Desktop browser viewport; mobile UX rendered inside a phone-shaped frame on the page
- Partner branding override via CSS custom properties (colors, fonts, logo)

## Issue Tracking

- All work is tracked via **GitHub Issues** on the `kcyr-greendot/cash-loads-demo` repository.
- Every commit must reference an issue number in the commit message (e.g., `closes #12` or `refs #7`).
- Claude may create GitHub Issues, but must get user approval before doing so.
- Before starting any new piece of work, confirm which issue it belongs to (or create one first).
