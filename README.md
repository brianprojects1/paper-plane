# Paper Plane

Send files straight from your browser to someone else's browser. Free, no accounts, no cloud storage, no size limit.

This is **one file**: `index.html`. Put it on GitHub Pages and you are done. No extension, no settings.

## Features

- Send one or several files, each gets its own link
- Optional password (with a generator button), max. 5 wrong attempts then locked for 15 minutes
- Link valid for 1 hour, 1 day or 7 days
- Stop automatically after 1, 3 or 10 downloads
- Files of any size (the receiver streams to disk; use Chrome or Edge for files over ~1.5 GB)
- Downloads resume automatically if the connection drops
- Live progress, speed and time left on both sides
- Light and dark theme
- "Check connection" chip that tests all connection services, and a details log on every link

## Important to know

- **The sender must stay online.** Keep the Paper Plane tab open and the computer awake until the recipient is done. Nothing is stored anywhere else.
- Setting up a connection uses three free public relays at the same time (ntfy.sh, HiveMQ, EMQX). Only tiny connection messages go through them, never the file. One working relay is enough.
- Very rarely a direct connection is impossible (strict firewalls). Another network, such as mobile data, usually fixes it.
- In Chrome, turn off Memory Saver for long transfers (`chrome://settings/performance`), or add the Paper Plane page to "Always keep these sites active".

## Using it

Open the page, drop a file, optionally set a password, expiry and download limit, and click **Create link**. Check that the link card shows a green dot and "Ready". Send the link to the recipient (send the password through another channel). Keep the tab open until they are done.

## If something does not work

1. Click the **Connected** chip at the top. Every service should show a tick. If all show a cross, your internet or a firewall blocks the relays.
2. Open **Details** on the link card. It shows each step, for example "Connection request received", "Answer sent".
3. On the receiver page, open **Details** too. Send me both logs if it still fails.
