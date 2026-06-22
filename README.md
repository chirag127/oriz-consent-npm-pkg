# @chirag127/oriz-consent

[![npm](https://img.shields.io/npm/v/@chirag127/oriz-consent.svg)](https://www.npmjs.com/package/@chirag127/oriz-consent)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE)

Klaro-based consent manager covering EU GDPR + UK + India DPDP + US GPC (Global Privacy Control) signals. Cookie banner + preference center.

## Install

```bash
pnpm add @chirag127/oriz-consent
```

## Status

v0.1.0 is a slug-reservation stub. Real implementation lands when oriz apps consume it.

## Planned API

- `mount({ services, locale })` — render the Klaro-backed banner + preference center.
- `getConsent(service)` — boolean check for any registered service (analytics, ads, etc.).
- `onChange(cb)` — subscribe to consent changes; fires after the user updates preferences.
- Auto-detects `navigator.globalPrivacyControl` and treats it as opt-out for US users.
- Multi-jurisdiction defaults: GDPR (opt-in), DPDP (opt-in), GPC (opt-out), UK PECR.

## License

MIT (c) 2026 Chirag Singhal
