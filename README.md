# Crystal Castles — browser-only architecture

ПК не требует установки программ. GitHub Pages hosts index.html and phone.html. A separate HTTPS/WSS signaling service is required to relay phone orientation to the PC browser.

PC: `index.html?server=wss://YOUR-SERVER&room=main`
Phone: `phone.html?server=wss://YOUR-SERVER&room=main`

The current original scene is preserved. The networking layer is the next step: deploy a tiny WebSocket relay, then wire the URL into index.html.
