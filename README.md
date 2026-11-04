# CIMB Live Rate (SGD-MYR)

**A live CIMB SGD-MYR exchange rate monitor**

An independent Chrome extension for keeping an eye on CIMB’s public indicative SGD-to-MYR quote from your toolbar. This repository is the public support and feedback hub.

## Get help or suggest an improvement

[Report a bug or suggest a feature](https://github.com/kelvinnivlek-sg/cimb-live-rate/issues/new)

Please include your Chrome version, extension version, what happened, what you expected, and the approximate time and timezone. Screenshots can help, but remove personal details first. Check existing issues before opening a new one.

GitHub Issues are public. Do not post bank details, phone numbers, identification documents, passwords or one-time codes.

## Features

- View a compact rate on the pinned toolbar icon.
- Hover or open the popup for the exact source quote and CIMB timestamp.
- Estimate an SGD-to-MYR conversion locally.
- Refresh manually whenever needed.

The compact badge truncates to two decimals without rounding up: 3.1565 appears as 3.15. The popup and tooltip retain the source quote’s precision.

## Automatic refresh

All scheduling uses Singapore time (UTC+8), independent of your computer timezone.

| Period | Check interval |
| --- | --- |
| Monday–Friday, 09:00–18:00 | Approximately every minute |
| Evenings, overnight and weekends | Approximately every five minutes |

Public holidays follow the normal weekday schedule. Chrome must be running; sleep, scheduling delays, network problems or source restrictions may prevent timely checks.

The extension keeps one inactive pinned CIMB public-rate tab open and refreshes that same tab. The source tab remains visible and may show a loading indicator. This is not a continuous streaming feed or a supported CIMB API.

## Troubleshooting

**No rate or a cached-rate warning:** check whether the pinned CIMB source tab loaded successfully. Try opening https://www.cimbclicks.com.sg/sgd-to-myr and using Refresh rate in the extension.

**Toolbar rate is not visible:** open Chrome’s Extensions menu (puzzle-piece icon) and pin the extension.

**The rate differs from a transfer quote:** the source rate is indicative. Always check the source timestamp and the actual quote in CIMB before making a transfer.

## Privacy policy

Last updated: 5 November 2026.

Publisher: [kelvinnivlek-sg](https://github.com/kelvinnivlek-sg). For privacy questions that do not involve sensitive information, open an issue in this repository. Do not post private financial or identity information publicly.

### Information stored locally

The extension stores the most recent public exchange rate, exact source rate text, CIMB source timestamp, time of the last successful check, and refresh error locally in Chrome. Calculator amounts stay in popup memory and are not stored or transmitted.

### Access to CIMB

The extension reads the public quote and source timestamp at https://www.cimbclicks.com.sg/sgd-to-myr. It creates or reuses one inactive pinned source tab and refreshes it according to the schedule above. It can also capture the quote when you manually open that public page.

Chrome handles normal website requests and cookie rules. Requests disclose ordinary connection information, such as your IP address, to CIMB under its policies. The extension does not read cookies, bank credentials or account balances and does not perform transfers.

### Sharing, analytics and removal

There is no developer analytics server, advertising or remote executable code. The extension does not transmit locally stored quote data to the developer. Images and executable code are bundled locally. Uninstalling the extension removes its local storage.

### Optional support

No financial-support destination is configured in version 1.0.0; the optional contribution link is hidden. All features are free.

## Independence

This project is not affiliated with, endorsed by or produced by CIMB. CIMB’s name and marks belong to their respective owner. Displayed rates are indicative and may differ from the final transfer quote.
