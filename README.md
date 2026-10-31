# Jayden's Quiz Quest

A quiz game for a 3rd grader: shapes, subtraction, multiplication and division.
It is one static page (`index.html`), so Vercel hosts it with no build step.

## Multiplayer (draft)

* Jayden's device becomes the host after entering the admin PIN on the start screen (tap "I'm Jayden").
* Guests pick a mission, choose Multiplayer, type their name and the room password, and join Jayden's room.
* Settings live at the top of the multiplayer code in `index.html` (search for `const CONFIG`):
  `ADMIN_PIN`, `ROOM_PASSWORD`, `FIREBASE`, `Q_TIME`, `REVEAL_TIME`.
* Until `FIREBASE` is filled in, multiplayer runs in demo mode (tabs on the same device only).
  Add `?guest=1` to the link to open a tab as a guest.
* `database.rules.json` holds the Firebase Realtime Database rules to paste into the Firebase console.

## Rolling back

The version from before multiplayer is saved on the `backup-2026-10-30-825pm` branch.
