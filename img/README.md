# Page artwork

`index.html` works without any of these files. Each one is a slot: drop the file in
with the exact name and the page picks it up automatically (no HTML edits needed).

| File | Where it appears | Notes |
|------|------------------|-------|
| `device.png` | Hero, right-hand column | Product photo. Replaces the data-flow diagram once present. Transparent background works best; roughly square. |
| `mb1.png` | Device Console viewer, tab 1 — *General* | Full-window screenshot of the console. |
| `mb2.png` | Device Console viewer, tab 2 — *Network* | |
| `mb3.png` | Device Console viewer, tab 3 — *Modbus & MQTT* | |
| `mb4.png` | Device Console viewer, tab 4 — *Live data* | Register values / sample log tables. |

The screenshot viewer stays hidden until at least one `mb*.png` exists, and each tab
only appears if its own file loads — so you can add them one at a time.

Captions and the fake URL bar text live in the `SHOT_CAPS` object near the bottom of
`index.html`; adjust them to match whatever you actually capture.
