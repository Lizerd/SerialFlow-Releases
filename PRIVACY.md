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

**What is kept:** the server adds each count to daily totals (for example "312 active installs, 840 hours, 6 Nov")
and throws the report itself away. Your IP address is not stored.

**Who handles it:**
- The counts are received by a Cloudflare Worker on lizerd.se and stored in Cloudflare D1.
- Cloudflare processes the web traffic as the hosting provider.
- GitHub handles downloads and issues under its own privacy policy.

**Changing your mind:** Settings → About → "Send anonymous usage counts".

## 3. Contact

Questions: https://github.com/Lizerd/SerialFlow-Releases/issues

*Last updated: 6 November 2026.*
