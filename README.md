# Bharat Internet Doctor — Cyber Safety Console

A privacy-first static webpage for quick, local URL/domain/IP structure checks and security guidance.

## Run

Open `index.html` in a modern browser or serve this directory with any static web server. No build step, backend, dependencies, API key, or GPU is required.

## What the local check does

- Parses an HTTP(S) URL, domain, or IP address in the browser.
- Shows the scheme, host type, and basic URL-structure signals (for example, HTTP, URL user-info, punycode, or unusually long input).
- Uses deliberately simple heuristics. Its “caution” label is not a threat verdict or a probability of compromise.
- Can copy a report only when the user explicitly clicks the button.

The tool does not open/fetch the target, scan ports, query WHOIS/DNS/reputation services, estimate hosting location, identify visitors, detect malware, or contact authorities. Private/local IP checks are informational only.

## Privacy and security boundaries

The page has no analytics, cookies, login, database, external scripts, API calls, or browser persistence. Inputs are processed in memory in the page. Copying a report is user-triggered. The hosting provider may independently process normal HTTP request metadata; consult its policy for server-side logging.

A normal website cannot silently inspect device files or provide continuous antivirus protection. For malware detection and 24/7 monitoring, use trusted endpoint security software installed with the device owner’s consent. Do not put secret API keys in frontend code. Any future external reputation/WHOIS/hosting integration should disclose what is sent, require explicit opt-in, label data provenance and confidence, and avoid automated accusation/reporting. Reports should remain user-reviewed and evidence-based.

For India cybercrime reporting information, use the official [National Cyber Crime Reporting Portal](https://cybercrime.gov.in/). For financial cyber fraud, contact your bank and call 1930 promptly.
