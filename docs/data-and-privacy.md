# Data and privacy

This is a product-design summary, not a promise that all data stays on a device or a legal compliance certification. See the [live explanation](https://moona.fun/about#sent-title) and contact [hello@moona.fun](mailto:hello@moona.fun) with questions.

| Data | Current design |
| --- | --- |
| Birth details, full chat history, readings, and journal notes | Stored in the user's browser. Email sign-in does not sync them between devices. |
| Email account and sessions | Stored server-side for verification-code sign-in, account continuity, and the user's separate updates preference. |
| AI request context | Sent to the server and AI provider when that feature is used. This may contain personal text. |
| Accepted AI replies | Temporarily cached server-side to replay requests without charging twice. Replies may quote or paraphrase user input. |
| Usage identifiers | Used for quotas, billing controls, and request replay. They can be associated with a signed-in account. |

Ordinary AI replies currently default to a two-hour cache; shared Sun-sign daily replies are about a day, and paid-reading paths have a longer default. Expired replies are removed by housekeeping, not necessarily erased at the exact expiry second. Database backups have a separate retention period, currently configured by the deployment's backup process with a 14-day default. A deleted live record may remain in a backup until that backup expires. Provider-side retention is governed separately by the services used.

Users can export or clear their device records, and the account settings provide an email-account deletion action. These actions have different scopes: clearing a browser does not erase server records, and deleting an email account does not instantly erase every backup or accounting record.

Please send private support requests by email, rather than posting personal information, verification codes, or conversation transcripts in public GitHub issues.
