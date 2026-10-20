Genesys Schedule Helper — Mobile Web v0.1.2 TEST

FIX: Test full alarm previously called unlockAudio() from another script's private scope,
raising ReferenceError and stopping the button handler. It now invokes the exported alarm
engine directly from the click. Scheduled alerts use the same alarm engine.

Settings: kept timing, sound, volume, Test full alarm, and Local data / Clear schedule.
Removed the extra version text below settings. Added author credit to dashboard.

UPDATE GITHUB PAGES:
Extract and upload all files to repository root, replacing existing files.
Commit changes, wait for Pages to publish, then refresh the phone browser.
If installed as a home-screen app, close it fully and reopen after updating.

Test: open Settings, select Digital alarm, volume > 0, tap Test full alarm.
The visible alert should open and sound repeat until dismissed.

Mobile browsers cannot guarantee sound while locked or backgrounded.
QR camera still depends on BarcodeDetector support.
