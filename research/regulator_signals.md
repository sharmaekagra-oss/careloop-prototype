# Regulator signals — why the "why now" holds

*The strongest "why now" claim is not that the problem is new — it's that **the regulator has publicly agreed it is a problem and is actively building the fix.** The fix isn't landing at scale yet. The gap is the opportunity.*

---

## RBI / NPCI moves on offline & low-connectivity UPI

### UPI Lite (2022 → 2024/25 limit expansion)
- Small-value, on-device UPI wallet. Pre-loaded while online; small payments then go without PIN or, in some flows, without live network.
- **Dec 2024:** RBI raised UPI Lite per-transaction limit to ₹1,000 and wallet cap to ₹5,000; updated the offline-payments framework.
  - Source: Business Standard, "RBI enhances UPI Lite wallet limits, updates offline payments framework" (Dec 2024) — https://www.business-standard.com/finance/news/rbi-enhances-upi-lite-wallet-limits-updates-offline-payments-framework-124120401144_1.html

### UPI Lite X — NFC tap-to-pay, fully offline
- Extension of UPI Lite using NFC for tap-to-pay. Capped at ₹2,000 per transaction initially.
- Use cases NPCI has publicly cited: aircraft cabins, underground metros — i.e., "places with no signal."
- Timeline: NPCI **certifying PoS terminals from major manufacturers in 2026**; rollout planned by **end of 2026.**
- Sources:
  - Deccan Herald, "NPCI developing offline UPI feature for payments without internet" — https://www.deccanherald.com/technology/npci-developing-offline-upi-feature-for-payments-without-internet-4082826
  - MediaNama, "NPCI Develops Offline UPI Payments for PoS Terminals" (Jul 2026) — https://www.medianama.com/2026/07/223-npci-offline-upi-nfc-pos-payments-tap-to-pay/
  - Outlook Business — https://www.outlookbusiness.com/corporate/upi-offline-mode-npci-building-nfc-tap-to-pay-for-flights-underground-trains

### UPI 123Pay — for feature phones, no internet
- Launched Mar 2022 by RBI + NPCI. Four flows: IVR calls, missed-call, OEM/app-based, sound-based proximity.
- Target market: **India's ~400 million feature phone users.**
- Per-transaction limit raised from ₹5,000 → ₹10,000.
- Sources:
  - IndBiz, "RBI launches UPI 123Pay for digital payments on feature phones" — https://indbiz.gov.in/rbi-launches-upi-123pay-for-digital-payments-on-feature-phones/
  - MicroSave, "UPI 123Pay: the four-leaf clover for feature-phone-based payments in India" (Oct 2023) — https://www.microsave.net/2023/10/10/upi-123pay-the-four-leaf-clover-for-feature-phone-based-payments-in-india/
  - Razorpay blog — https://razorpay.com/blog/what-is-upi-123-pay/

### RBI-approved offline rails (bank-specific)
- **HDFC OfflinePay** — RBI approval received. One example of a bank rolling out its own offline flow.
  - Source: Outlook Money, "UPI Offline Payment Methods: RBI Announces Approval for HDFC's OfflinePay" — https://www.outlookmoney.com/banking/upi-offline-payment-methods-rbi-announces-approval-for-hdfcs-offlinepay

---

## What the "why now" line reads as

> The Reserve Bank of India has been raising UPI Lite limits, approving bank-specific offline rails, and instructing NPCI to certify NFC tap-to-pay PoS terminals through 2026. **The regulator agrees.** But adoption of the offline rails is still a rounding error against on-line UPI volume — 21.63 billion monthly txns in Dec 2025 vs. an offline stack that only NPCI's PR desk mentions. **The gap between the fix being built and the fix being felt is where the opportunity sits.**

---

## The "cash paradox" — a critical framing point

RBI Deputy Governor **Shirish Chandra Murmu** has publicly noted: digital payments in India are **additive, not substitutive** — cash usage share is declining but absolute currency-in-circulation is still climbing at double-digit rates.

Implication for our problem: users are NOT replacing cash with digital. They are stacking digital on top of cash — but the young / urban / power-user cohort **has quietly stopped carrying cash** (see Aariz Ahmed in `outage_coverage.md`). That cohort is where the UPI-lockout pain is sharpest. The "cash paradox" statistic looks reassuring at the population level and disguises a very sharp painpoint at the cohort level.

Sources:
- CryptoBriefing summary of Murmu's remarks — https://cryptobriefing.com/india-cash-paradox-digital-payments/
- DTNext / LatestLY on the RBI economist study — https://www.dtnext.in/news/business/cash-transactions-decline-rapidly-in-india-as-digital-payments-surge-rbi-economist-808507
- IBEF summary — https://www.ibef.org/news/digital-payments-double-in-three-years-cash-transactions-fall-reserve-bank-of-india-rbi-report

---

## Cash-share timeline (from RBI's Cash Usage Indicator)

- Q1 2021 — cash = **81–86%** of consumer expenditure
- Q1 2024 — cash = **52–60%** of consumer expenditure
- Same period — share of digital in payments doubled from 14–19% (Mar 2021) to 40–48% (Mar 2024)

Same sources as above.
