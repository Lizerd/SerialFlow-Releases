# SerialFlow privacy

**Short version:** SerialFlow does not know who you are. It can check for updates, and if you agree it sends one
anonymous count a day. Nothing about your devices, ports or data ever leaves your PC.

## 1. Update check (on by default, can be turned off)

When SerialFlow starts, it downloads `https://lizerd.se/serialflow/latest.json` to see whether a newer version
exists. It sends nothing except the normal web request. If you choose to update, the new version is downloaded from
GitHub (`github.com/Lizerd/SerialFlow-Releases`).

## 2. Anonymous usage count (only if you say yes)

At first start SerialFlow asks whether it may send an anonymous count. If you agree, it sends this at most once a
day:

| Sent | Example |
|---|---|
| App version | `0.9.0-beta.1` |
| Windows version (major only) | `win11` |
| Channel | `beta` |
| Minutes the app was open since the last count | `95` |
| First count from this PC today / this week / this month / ever | `true` / `false` / `false` / `false` |

**What it does not send:**
- no user or install ID, no computer name, user name or hardware fingerprint
- nothing about your serial ports, devices, logs, graphs or settings

**What is kept:** a small script on lizerd.se adds each count to daily totals (for example "312 active installs,
840 hours, 10 Nov") and throws the report itself away. The script stores no IP address and no ID.

**Who handles it:**
- lizerd.se is hosted by Hostup in Sweden, with Cloudflare in front. The update check and the daily count pass
  through them like any visit to the website, and the web host keeps standard access logs (which include IP
  addresses) under its own policy.
- GitHub handles downloads, updates and issues under its own privacy policy.

**Changing your mind:** Settings → About → "Send anonymous usage counts".

## 3. Contact

Questions: https://github.com/Lizerd/SerialFlow-Releases/issues

*Last updated: 10 November 2026.*
