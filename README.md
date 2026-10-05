# ClutchPing

Low-latency tunnel for **Valorant / Riot Games / Discord** — Windows app, one file.

* **Download:** [`ClutchPing.exe` from the latest release](../../releases/latest). No installer. Windows SmartScreen will warn
  once because the exe is not code-signed: *More info → Run anyway*.
* **Needs:** Windows 10/11 64-bit, administrator (it creates the "ClutchPing" network adapter — kernel WireGuard via the
  WireGuardNT driver, the same one the official WireGuard app uses). Vanguard is fine with it.
* **Profile:** you need a `profile.json` (or `.conf`) with your personal key for the server. Put it next to the exe the
  first time; it is copied to `%LocalAppData%\ClutchPing` and kept through updates.
* **Updates:** TOOLS › CHECK / UPDATE NOW inside the app — it downloads the newest release from here, swaps itself and restarts.

Pick **Valorant** and/or **Discord** → **CONNECT** → start the game / Discord. Only their traffic goes through the tunnel
(Riot's game and voice servers by address block, everything else host by host as the whitelisted domains resolve); the
browser and everything else on the PC stay direct.
