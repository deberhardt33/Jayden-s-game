# Jayden's Quiz Quest

A quiz game for a 3rd grader: shapes, subtraction, multiplication and division.
It is one static page (`index.html`), so Vercel hosts it with no build step.

## Multiplayer (draft)

* After picking a mission and Multiplayer, the game asks "Are you Jayden?". Yes asks for the 4 digit PIN and makes him the host. No asks for a name and the room password.
* Single player never asks who you are.
* Settings live at the top of the multiplayer code in `index.html` (search for `const CONFIG`):
  `ADMIN_PIN`, `ROOM_PASSWORD`, `FIREBASE`, `Q_TIME`, `REVEAL_TIME`.
* Until `FIREBASE` is filled in, multiplayer runs in demo mode (tabs on the same device only).
* `database.rules.json` holds the Firebase Realtime Database rules to paste into the Firebase console.

## Rolling back

The version from before multiplayer is saved on the `backup-2026-10-30-825pm` branch.
