# Sizing — the scale of what breaks when it breaks

*Every number here is from an official / mainstream source, cited. No Statista TAM chest-thumping.*

---

## UPI monthly transaction volumes (NPCI data, via press)

| Month | Volume (billion txns) | Value |
|---|---|---|
| Jun 2025 | 18.39 | ₹24.03 lakh crore |
| Jul 2025 | 19.47 | ₹25.1 lakh crore |
| Aug 2025 | 20.01 (first month > 20B) | ₹24.85 lakh crore |
| Oct 2025 | — | **₹27.28 lakh crore** (value record at the time) |
| Nov 2025 | +32% YoY | — |
| **Dec 2025** | **21.63 (all-time high)** | **₹27.97 lakh crore** |
| Jun 2026 | 22.72 | ₹28.92 lakh crore |

**Full-year 2025:** 228.3 billion UPI transactions vs. 131.13 billion in 2024 — **~74% YoY growth.**

Daily average recently: **707 million UPI transactions per day** (Aug 2025 milestone).

Sources:
- BusinessStandard, "UPI transactions hit record 19.47 billion in July 2025" — https://www.business-standard.com/amp/markets/capital-market-news/upi-transactions-hit-record-19-47-billion-in-july-2025-cross-rs-25-lakh-crore-in-value-125080200723_1.html
- Elets BFSI, "UPI Smashes Records with 21.6 Billion Transactions in December 2025" — https://bfsi.eletsonline.com/upi-smashes-records-with-21-6-billion-transactions-in-december-2025/
- News on Air, "UPI records all-time high in July with 19.47 crore transactions worth ₹25.1 lakh cr" — https://www.newsonair.gov.in/upi-records-all-time-high-in-july-with-1947-cr-transactions-worth-%E2%82%B925-1-lakh-cr
- News on Air, "UPI sets new record with 707 million daily transactions" (Aug 2025) — https://www.newsonair.gov.in/upi-sets-new-record-with-707-million-daily-transactions
- News on Air, "UPI transactions increase by 32% in November" — https://www.newsonair.gov.in/upi-transactions-increase-by-32-in-november-data-released-by-npci
- Business Standard on Oct 2025 record — https://www.business-standard.com/economy/news/upi-transactions-hit-record-high-of-rs-27-28-lakh-crore-in-oct-125110300839_1.html

---

## UPI share of India's retail digital payments

- **H2 2025** — UPI = **85.5%** of digital payment transaction volume (RBI report).
- **FY24–25** — UPI = **81%** of all retail digital payments (RBI).
- UPI accounts for **~49% of global real-time payment transactions** (IMF, cited by PIB).
- **500+ million unique UPI users** by early 2026 (up from ~420M cited earlier).

Sources:
- IBEF, "UPI accounted for 85.5% of digital transaction volume in H2 2025: RBI report" — https://www.ibef.org/news/upi-accounted-for-85-5-of-digital-transaction-volume-in-h2-2025-rbi-report
- DD News on the same RBI report — https://ddnews.gov.in/en/upi-accounted-for-85-5-of-digital-transaction-volume-in-h2-2025-rbi-report/
- Tech Observer, "UPI drives 81% of India's digital payments" — https://techobserver.in/news/egov/upi-digital-payments-india-22000-crore-transactions-2025-321551/
- PIB, "UPI Recognized as World's Largest Real-Time Payment System by IMF; Accounts for 49% of Global Transactions" — https://www.pib.gov.in/PressReleasePage.aspx?PRID=2200569
- CoinLaw, "UPI Statistics 2026: India's Real-Time Payments Decade" — https://coinlaw.io/upi-statistics/
- BCG India UPI report 2025 — https://www.bcg.com/publications/2025/india-upi-the-global-benchmark-for-digital-payments

---

## Cash trajectory

- Cash share of consumer expenditure: **81–86% (Q1 2021) → 52–60% (Q1 2024).** RBI Cash Usage Indicator.
- Digital share: **14–19% (Mar 2021) → 40–48% (Mar 2024).**
- But: absolute currency-in-circulation growing at double-digit rates (RBI Deputy Governor Murmu — the "cash paradox").

Sources (same as `regulator_signals.md`).

---

## Telecom outage frequency (India)

Not a single official stat, but at minimum the following are documented in mainstream Indian press over the last 24 months. This is a floor, not a ceiling:

- Reliance Jio nationwide outage — 17 Sep 2024
- Airtel multi-city outage — 11 Feb 2025 (5–10 min official, longer for users)
- UPI outage — 26 Mar 2025
- UPI outage — 2 Apr 2025
- UPI outage — 12 Apr 2025 (~5 hours)
- Airtel multi-city outage — 24 Aug 2025 (6,800+ complaints peak)
- Airtel Delhi-NCR outage — Jun 2026

Sources: as per `outage_coverage.md`.

---

## What the sizing tells us for the JTBD

Rough back-of-envelope of pain surface area (all defended by citations above):

- **~22 billion txns/month** run through UPI as of mid-2026.
- **UPI is 85%+ of digital retail volume.**
- Even a **0.1% failure rate** = ~22 million failed transactions per month.
- A single 5-hour national outage (Apr 12 2025) affected **all three major apps** — every UPI user in the country was locked out at once.
- **500M+ users** carry UPI as their default; the young/urban/power-user sub-segment has stopped carrying cash entirely (see Aariz Ahmed quote).
- Every one of the outages above is also a **payment lockout event** for the sub-segment that has decoupled from cash.

This is not a rare event. This is an ambient, structural feature of building the world's largest real-time payments system on top of one SIM, one signal, one phone.
