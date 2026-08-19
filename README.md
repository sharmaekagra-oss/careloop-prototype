# CareLoop — patient prototype

Interactive prototype for the CareLoop design sprint (Team 7, MICA Design Sprint Studio).
Built for user testing: a tester plays **Radha, 58**, managing hypertension and type 2
diabetes at home.

It is a single self-contained `index.html` — no build step, no dependencies, no backend.
Everything runs in the browser and saves to `localStorage`.

## Running it

Open `index.html` in a browser, or serve the folder:

```bash
python -m http.server 5500
```

Then visit `http://localhost:5500`.

## Two URLs

| URL | Who it's for | What they see |
| --- | --- | --- |
| `/` | **Test users** | The patient app only |
| `/#facilitator` | **You, running the session** | Adds a role switcher (Caregiver / Clinic / Doctor) and facilitator controls |

Send testers the plain URL. Keep `#facilitator` for yourself.

## What it demonstrates

- **Clinic-led onboarding** — six steps, including the AI voice choice and consent toggles
- **Tiered adherence** — on track stays silent, a first miss nudges gently, a pattern
  (or any miss on a high-risk medicine) triggers an AI check-in call that really speaks,
  using the browser's speech synthesis
- **Escalation** — declining the call notifies the caregiver; a weekly pattern reaches the
  clinic; the doctor gets exceptions, labelled as self-reported rather than observed
- **Contrast mode** — replays the same day as a typical ping-every-dose reminder app.
  On an identical compliant day: 2 notifications versus 11
- **Refill tracking** — warns before a medicine runs out, not after
- **Why a dose was skipped** — *forgot* / *feeling better* / *side effect*. "Feeling better"
  shows why the course continues instead of nagging; a side effect reaches the clinic
- **Missed OPD slot** — flagged to the clinic with waitlist recovery

## The simulation rail

A day passes faster than real time. The dashed strip above the phone is scaffolding, not
product — use **Skip to next moment** to advance to the next dose or deadline.

## Notes for testing

- **Sound on.** The check-in call and instruction note are spoken aloud.
- The voice comes from the tester's own device, so it differs between phones. Devices
  without an Indian English voice fall back to the nearest English one.
- If speech is unavailable, the call still shows its full script as text — the flow never
  blocks.
- Each tester's session is independent. *Settings → Start the test over* resets everything.

## Deploying

Any static host works, since there is nothing to build. Point it at this folder and serve
`index.html`.
