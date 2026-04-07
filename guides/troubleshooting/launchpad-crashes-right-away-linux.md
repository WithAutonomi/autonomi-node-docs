---
description: >-
  Some Linux users experience Launchpad crashing a second after launching it.
  But have no fear, we have a fix for you!
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/mHMagc6BlRPNTxTKcyjL/guides/troubleshooting/launchpad-crashes-right-away-linux
---

# Launchpad crashes right away - Linux

1. Show Hidden Files in File Manager

Linux hides certain folders by default. Here's how to reveal them:

* Open your **File Manager** (e.g., Files, Dolphin, Nautilus).
* Click the **three-line “hamburger” menu** or find the **View** menu.
* Select **"Show Hidden Files"**.

&#x20;Or press `Ctrl + H` while inside the file manager to toggle hidden files on/off.



2. From your home directory, navigate to `.local/share/autonomi/` You should see folders and files related to the Launchpad inside.



3. Delete the Autonomi folder&#x20;

* In your file manager go to `/home/YOUR_USERNAME/.local/share/`
* Find the `Autonomi` folder&#x20;
* Right-click and select **Delete**, or select it and press the **Delete** key. This sends it to the Trash. Now empty the Trash to remove it completely.



4. Reinstall[ Launchpad](https://docs.autonomi.com/node/downloads)&#x20;



