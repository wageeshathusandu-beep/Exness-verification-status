# Verification Status — Demo Dashboard

A clean, premium dark-UI document & address verification status dashboard. **This is an
independent demonstration and is not an official Exness service.**

## What it shows

### Document Verification — Completed ✅
  1. Upload Documents — Completed ✅
  2. Document Processing — Completed ✅
  3. Verification Status — Completed ✅
- A prominent green **Completed** badge with a checkmark.
- A professional **progress timeline** (horizontal on desktop, vertical on mobile) with all 3 steps complete.
- Status message:

  > Your identity documents have been verified successfully.

### Address Verification — Interactive workflow
Once document verification is complete, an **Address Verification** section appears automatically:

1. **Upload** — drag & drop or browse proof-of-address documents.
   - Accepted document types: utility bills, bank statements, official address documents.
   - Accepted formats: **JPG, PNG and PDF** (up to 10MB each).
   - Multiple document uploads supported, with live image/PDF previews and per-file removal.
2. **Submit** — click *Submit for Verification* (enabled once at least one file is added).
3. **Pending** — after submission:
   - A success notification is shown.
   - Address Verification status changes to **Pending Verification** (yellow clock icon).
   - Message: *Your address documents have been submitted and are currently under review.*
   - Submission date, time, reference ID, and document list are displayed and persisted.
   - The status stays pending until an authorized reviewer approves it.
4. **Approval (demo only)** — a *Simulate Approval* control lets a reviewer approve the address verification, after which the status turns green (Verified). A *Reset Workflow* control restores the upload state.

## Features

- Single self-contained `index.html` (no build step, no external dependencies).
- Premium dark theme with glassmorphism cards and subtle glow accents — green for completed, gold/amber for pending.
- Fully functional state machine: upload → submit → pending → (simulated) approval.
- Client-side persistence (localStorage) simulates secure backend storage: uploaded documents, submission timestamp, and status survive page reloads.
- Drag & drop uploads with validation (format & size), image thumbnails, and PDF placeholders.
- Smooth animations and transitions throughout, with reduced-motion support.
- Fully responsive: timeline, document-type chips, preview grid, and toast all adapt to mobile.
- Accessible: semantic landmarks, `aria-live` status regions, keyboard-operable dropzone.

## Usage

Just open `index.html` in any modern browser. No server required.

> **Demo mode:** verification approval is simulated entirely in your browser. No documents leave your device.

## Disclaimer

This dashboard is a demonstration created for illustrative purposes only. It is
not affiliated with, endorsed by, or connected to Exness. All reference IDs and
statuses shown here are sample data.
