# Outage coverage — the fragile last mile

*Every claim traceable via URL. Only material I could verify through search snippets is included. Full-article paywalls / SPA pages were not directly fetchable from this session's network.*

---

## The three UPI outages of 2025 (the "why now" anchor)

Three UPI outages inside 17 days, spring 2025.

- **26 March 2025** — outage #1.
- **2 April 2025** — outage #2, roughly a week later.
- **12 April 2025** — outage #3. **~5 hours downtime, the longest in recent years.** Affected Google Pay, PhonePe, Paytm.

**Root cause (per NPCI's RCA):** PSP banks flooding the network with "check transaction status" API calls at unsustainable TPS, overwhelming capacity.

**NPCI response (Apr 2025):** New guidelines to PSP banks — status-check calls only after 90 sec, capped at 3 checks per 2-hour window per transaction.

Sources:
- MediaNama, "NPCI Restores UPI After Nationwide Payment Failures" (Apr 2025) — https://www.medianama.com/2025/04/223-npci-upi-outage-april-12-2025/
- MediaNama, "NPCI Issues New Guidelines to Curb UPI Outage" (Apr 2025) — https://www.medianama.com/2025/04/223-npci-new-guidelines-upi-outage/
- India TV News, "UPI outage caused due to certain banks, says NPCI" (16 Apr 2025) — https://www.indiatvnews.com/technology/news/upi-outage-caused-due-to-certain-banks-says-npci-as-it-plans-fixes-2025-04-16-985701
- Kapronasia, "UPI outages in early 2025 indicate need for tighter controls and monitoring" — https://www.kapronasia.com/asia-payments-research-category/upi-outages-in-early-2025-indicate-need-for-tighter-controls-and-monitoring.html
- ORF, "UPI at Scale: Outages and the Push for Resilient Systems" — https://www.orfonline.org/expert-speak/upi-at-scale-outages-and-the-push-for-resilient-systems

---

## The Bangalore BMTC bus story — the best named-user quote

May 2024. UPI on BMTC airport buses (partnered with Canara Bank's ETMs) failed for **two consecutive days**. Cash-only demanded by conductors. Two named commuters were quoted:

> **Rajesh Kumar**, regular BMTC airport-bus commuter, was forced to disembark mid-journey and hail an auto-rickshaw when the conductor said UPI was not functioning and insisted on cash — which he did not have.

> **Aariz Ahmed** said he was frustrated to have to get down mid-journey just because he didn't have cash, as he **"usually never carries cash and solely depends on digital payments."**

> *← This is a verbatim non-consumption confession from a named commuter, in a mainstream Indian daily. It is the strongest single quote for the PDF.*

Reported by Darshan Devaiah B for The Hindu-Bengaluru (10–11 May 2024).

Sources:
- The Hindu-Bengaluru, "Commuters face disruption as UPI payments fail on BMTC airport buses" (11 May 2024) — https://www.pressreader.com/india/the-hindu-bangalore-9WW1/20240511/281590950657475
- The Hindu-Bengaluru on X — https://x.com/THBengaluru/status/1789157293071683774

---

## The "Cash is always king" mainstream-narrative moment (Apr 2025)

Deccan Herald ran two pieces during the April 2025 outages compiling netizen reactions. Both articles' snippet-level content confirms:

- Netizens **explicitly** joked they had to "clean vessels at the restaurant" because they couldn't pay.
- One user compared themselves to the RBI governor, saying they had "**no control over our own money**."
- Multiple users converged on: **carry cash.**

Sources:
- Deccan Herald, "'Cleaned vessels at restaurant': UPI down in India, netizens up their meme game" (Mar/Apr 2025) — https://www.deccanherald.com/india/cleaned-vessels-at-restaurant-upi-down-in-india-netizens-up-their-meme-game-3465040
- Deccan Herald, "'Cash is always king': UPI down again, netizens share anecdotes" (Apr 2025) — https://www.deccanherald.com/business/cash-is-always-king-upi-down-again-netizens-share-anecdotes-3491157
- Deccan Herald opinion, "UPI outages call for stronger checks" — https://www.deccanherald.com/opinion/editorial/upi-outages-call-for-stronger-checks-3497272

---

## Telecom-side outages — the OTHER half of the fragile stack

UPI needs internet. Internet needs SIM/network. Every telecom outage is a UPI outage waiting to happen.

**Reliance Jio, 17 Sep 2024**
- Downdetector logged **10,000+ reports**.
- Outage began ~11 AM; peak throughout the afternoon; still ~1,500 active reports at 3:20 PM.
- Affected both Jio mobile and Jio AirFiber.
- Source: BusinessToday, "Reliance Jio faces major outage" (17 Sep 2024) — https://www.businesstoday.in/technology/news/story/reliance-jio-faces-major-outage-thousands-of-users-affected-446262-2024-09-17

**Airtel, 11 Feb 2025**
- Outage began ~11 AM. Multi-city: Bengaluru, Delhi, Jaipur, Indore, Kolkata, Chennai, Hyderabad.
- Airtel officially: "disrupted for approximately five minutes… fully normalized within the next 10 minutes" (users' lived experience of the disruption was longer).
- Source: Deccan Herald, "Airtel cellular internet service down in multiple cities" — https://www.deccanherald.com/technology/airtel-cellular-internet-service-down-in-multiple-cities-in-india-1080374.html

**Airtel, 24 Aug 2025**
- Delhi, Mumbai, Bengaluru, Hyderabad, Chennai, Kolkata.
- Peak at 12:11 PM with **6,800+ complaints**.
- **52% cited "No Signal", 31% cited mobile data failure.**
- Source: BusinessToday (24 Aug 2025) — https://www.businesstoday.in/amp/india/story/airtel-outage-hits-major-indian-cities-users-report-call-and-internet-disruptions-490838-2025-08-24
- Source: WION News — https://www.wionews.com/india-news/airtel-network-outage-hits-multiple-cities-in-india-bengaluru-hyderabad-and-chennai-worst-affected-1756034640037

**Airtel, June 2026**
- Delhi-NCR, Mumbai, other urban centres. Overnight into Fri morning.
- **64% mobile internet, 27% signal, 6% voice.**
- Source: The Tribune, "Airtel network disruptions affect thousands across India" — https://www.tribuneindia.com/news/business/airtel-network-disruptions-affect-thousands-across-india/

---

## Adjacent structural pressure on the UPI stack (color, not core)

Even outside the network-outage story, UPI's last mile is fraying:

- **Aug 2026** — Tamil Nadu petrol pump associations threaten to stop accepting UPI over cybercrime-triggered bank-account freezes (mule-account flagging).
  https://www.medianama.com/2026/08/223-tamil-nadu-petrol-pumps-upi-boycott/
- **Sep 2026** — Petrol pump dealers nationwide threaten cash-only for ₹2,000+ transactions over the proposed ₹5 flat MDR.
  https://www.businesstoday.in/latest/economy/story/petrol-pump-dealers-oppose-rs5-upi-mdr-warn-of-cash-only-payments-for-big-transactions-555985-2026-09-16

*Read: even merchants — the last people in the UPI chain — are hedging back to cash under multiple, unrelated stress vectors. The fragile last mile is a system-level property.*
