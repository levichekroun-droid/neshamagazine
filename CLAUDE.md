# NeshamaGazine site: working rules

- `status.json` at the repo root is the "technician team at work" switch.
  - Before starting work on the live site: set `{"fixing": true, "msg": ""}`, commit and push it by itself.
  - When the work is done: push the new site together with `{"fixing": false, "msg": ""}`.
  - Every open page checks it every 15 seconds: while `fixing` is true visitors see the technician screen; when it turns false the page loads the new version.
- The owner can still get in while it shows: hold the gears for 3 seconds, or type "neshama".
