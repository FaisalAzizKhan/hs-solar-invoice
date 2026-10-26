# H & S Solar Energy - Solar Invoice Generator

A password-protected, static web page for creating H & S Solar Energy solar quotations / invoices as PDF.

**Open:** https://faisalazizkhan.github.io/hs-solar-invoice/

## How it works

- The whole app is encrypted (AES-256-GCM, key derived from the email + password with PBKDF2-SHA256, 600,000 iterations). The published `index.html` contains only a sign-in form and the encrypted data; nothing of the app can be read without valid credentials.
- Decryption happens in your browser. No server, no accounts database, no tracking.
- Everything you type (customer details, company settings, saved drafts) stays in your browser's local storage on your device. Nothing is uploaded.

## How to use

1. Open the link above (it must be the https link).
2. Sign in with your email and password. Tick **Remember me on this device** to skip the sign-in next time on this device.
3. Fill in the customer details and items.
4. Press **Generate & Download PDF**. On iPhone, use **Open PDF**, then Share -> Save to Files if the download does not start.
5. Use **Sign out** (top-right corner) to forget the saved sign-in on a shared device.

Credentials are shared privately by the owner; they are not stored in this repository.
