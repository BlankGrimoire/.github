# Security Policy

## Supported versions

BlankGrimoire is in early development. Only the latest release of each
repository receives security fixes.

| Component | Supported |
|---|---|
| BlankGrimoire-iOS: latest release | ✅ |
| BlankGrimoire-sdk: latest major | ✅ |
| BlankGrimoire-themes: latest published bundles | ✅ |
| Older versions | ❌ |

## Reporting a vulnerability

**Please do not open public issues, discussions or pull requests for
security problems.**

Report vulnerabilities privately through one of these channels:

1. GitHub **Private vulnerability reporting**: open the affected repository,
   go to **Security → Report a vulnerability**;
2. email: **pr3o.y@gmail.com**.

Please include:

- the affected repository and version;
- a description of the issue and its potential impact;
- steps to reproduce or a proof of concept;
- any suggested mitigation, if known.

## Our commitment

- We will acknowledge your report within **72 hours**.
- We will keep you informed about the progress of the fix.
- We will credit you in the release notes, unless you prefer to remain anonymous.

Please give us reasonable time to release a fix before any public disclosure.

## Scope

We are particularly interested in:

- escapes from the JavaScriptCore sandbox or abuse of the native bridge;
- bypasses of the per-site host allowlist;
- flaws in adapter bundle signature verification (Ed25519) or in the
  trust-on-first-use model for adapter repositories;
- leaks of cookies, session data or library data between sites or adapters;
- injection issues in scripts or content rules executed inside web views.

## Out of scope

- Vulnerabilities of third-party websites added by users.
- Requests to support, unblock or access specific websites.
- Issues requiring a jailbroken device or physical access to an unlocked device.