# Vessel Logbook

A simple offline-capable PWA for recording crew hours and sea service on near coastal small vessels, with exports aimed at AMSA sea service evidence.

- **Log** duty periods per vessel (position, AMSA duty code, operation type, underway / not underway).
- **Export → Logbook PDF**: full record with a sea service summary and duty list.
- **Export → Form 771 sheets**: one page per vessel / duty / operation type with the details needed for AMSA form 771 (not the official form itself).
- Day counting follows AMSA's near coastal rule: 1 day = 8 hours of relevant work; shorter shifts are combined; max one day per 24 hours.
- Data is stored in the browser (`localStorage`) only. Use Settings → Export backup regularly.

Run locally: `python3 -m http.server` and open `http://localhost:8000/`.

Always check current requirements on amsa.gov.au; area/duty codes and the 771 layout should be confirmed against the current AMSA form.
