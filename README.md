# KosherGuard category filter, staging handoff

All 28 switches implemented and tested. Limited or empty coverage is explicitly displayed. No deployment or production traffic enforcement.

## Get the development project

1. Download `2-kosherguard-category-development.tar.gz` and extract it.
2. Download `1-kosherguard-category-runtime.sqlite`.
3. Place the SQLite file at `artifacts/runtime.sqlite` inside the extracted project.
4. Read the project's README for Python requirements, local startup, tests, evidence and limits.

The runtime is 8,380,416 bytes with 298,304 unique exact hosts. SHA-256: `945aa64e25c6b6218b3bb3b9f451fe51893cb383a9f5d9c828369d9906edbdc6`.

24 automated tests pass. Browser tests cover 56 actual ON/OFF clicks, settings reload, original-control adapter and widths 320/390/1280. Every category shows its stored-host count plus limited or empty status. Expired threat records show zero current threat hosts and remain unresolved.

Five categories have no real assignments. Adult has one individually reviewed exact host. Bulk UT1 mappings remain provisional. Threat corroboration expires after five minutes and the packaged snapshot is expired. No automatic refresh service is running. Unknown and stale never mean safe. This is a category-decision app, not a DNS/HTTPS/phone traffic filter.

Full report: https://files.instinct.com/sn7ynf25ts55-kosherguard-category-filter-results (owner sign-in required).

The original full UT1 archive and full staging evidence are retained separately, not included here. Data notices and provenance ledger are included in the development archive. No live settings, credentials, management dashboard, device data or production configuration is included. Nothing was deployed or activated.
