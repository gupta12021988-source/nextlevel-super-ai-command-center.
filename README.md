# Bharat Internet Doctor

A privacy-first static security-awareness page for users in India. It is intentionally honest about what a normal website can and cannot do.

## What it does

- Checks whether the page is running in a secure browser context (usually HTTPS or localhost).
- Provides practical device-security guidance and links to official reporting resources.
- Runs entirely in the browser. The check makes no network requests and stores no results.
- Requires no login, database, analytics, or API key.

## What it does not do

A webpage cannot silently inspect all files on a visitor's device, run a complete antivirus scan, remove malware, or monitor the device 24/7. Browser sandboxing prevents this by design. This project does not identify visitors, collect their IP addresses, or send reports to authorities.

For actual malware detection and continuous protection, use trusted endpoint security software installed and authorized on the device. A future endpoint product would need a transparent, opt-in native agent, least-privilege permissions, a signed update process, clear uninstall controls, and a documented privacy policy. Do not put secret API keys in frontend code; server-side secrets require a secured backend. Any future reporting workflow should be evidence-based and user-reviewed before submission.

## Privacy note

The page itself has no analytics, cookies, login, database, scan API, or persistent browser storage. The hosting provider may independently process standard web request metadata; hosting-side logging is outside the page's control.

## Run locally

Open `index.html` in a browser, or serve this directory using any static web server. The secure-context check may report a non-secure context when opened directly as a `file://` URL; use HTTPS or localhost for a secure context.
