<div align="center">

```
██████╗  █████╗ ██████╗ ██╗  ██╗██████╗  ██████╗ ██████╗ ██╗  ██╗
██╔══██╗██╔══██╗██╔══██╗██║ ██╔╝██╔══██╗██╔═══██╗██╔══██╗██║ ██╔╝
██║  ██║███████║██████╔╝█████╔╝ ██║  ██║██║   ██║██████╔╝█████╔╝ 
██║  ██║██╔══██║██╔══██╗██╔═██╗ ██║  ██║██║   ██║██╔══██╗██╔═██╗ 
██████╔╝██║  ██║██║  ██║██║  ██╗██████╔╝╚██████╔╝██║  ██║██║  ██╗
╚═════╝ ╚═╝  ╚═╝╚═╝  ╚═╝╚═╝  ╚═╝╚═════╝  ╚═════╝ ╚═╝  ╚═╝╚═╝  ╚═╝
```

**Google Dork Query Builder · Bug Bounty Recon · OSINT Tool Library**

[![Live](https://img.shields.io/badge/live-0xcgz.github.io-111111?style=flat-square&logo=github)](https://0xcgz.github.io)
[![License](https://img.shields.io/badge/license-MIT-111111?style=flat-square)](LICENSE)
[![Dorks](https://img.shields.io/badge/dorks-100%2B-111111?style=flat-square)](https://0xcgz.github.io)
[![BB Queries](https://img.shields.io/badge/bb%20queries-60%2B-111111?style=flat-square)](https://0xcgz.github.io)
[![Tools](https://img.shields.io/badge/osint%20tools-20%2B-111111?style=flat-square)](https://0xcgz.github.io)
[![Made with](https://img.shields.io/badge/built%20with-vanilla%20html-111111?style=flat-square)](https://0xcgz.github.io)

</div>

---

## What is DarkDork?

**DarkDork** is a browser-based 3-in-1 recon toolkit. No backend, no login, no tracking — open it and start dorking.

Three modules in one file: a Google Dork builder, a Bug Bounty recon suite with external tool launchers, and a curated OSINT library. Pick a target domain, select a preset, and see the full query rendered live with syntax highlighting before you search.

---

## Modules

### 01 — Google Dorking
Live query builder with 100+ presets across 9 categories. Set a domain once and it auto-injects `site:` into every query.

### 02 — Bug Bounty Search
60+ recon queries targeting common bug bounty attack surfaces — exposed configs, login panels, vuln signatures, WordPress installs. Includes direct launchers for Shodan, crt.sh, Wayback Machine, Censys, GitHub, ThreatCrowd, Reddit, and more.

### 03 — OSINT Toolkit
20+ curated external intelligence platforms organized by category with one-click launch. Filtered by use case tab.

---

## Features

| Feature | Description |
|---|---|
| **3D Recon Globe** | Interactive particle network background — 250 nodes on a Fibonacci sphere, mouse-driven parallax, pulsing HVT nodes |
| **Target Domain Input** | Set a domain once — auto-injects `site:` into every Google dork |
| **Live Query Preview** | Syntax-highlighted preview with operator colouring before you search |
| **100+ Dork Presets** | Categorized: files, creds, login, vulns, iot, cloud, osint |
| **60+ BB Recon Queries** | Categorized: recon, files, vulns, login, docs, external |
| **External Tool Launchers** | Opens Shodan, crt.sh, Wayback, Censys, GitHub search and more directly |
| **OSINT Tools Library** | 20+ tools across 8 categories with one-click launch |
| **Live Search Filter** | Filter any dork by name or query string in real time |
| **Category Tabs** | Filter presets by type — all, files, creds, vulns, login, etc. |
| **Dark / Light Mode** | Toggles cleanly, preference saved to localStorage |
| **Copy to Clipboard** | One click copies the full raw query string |
| **Zero Dependencies** | Pure HTML/CSS/JS — no npm, no build step, no framework |
| **GitHub Pages Ready** | Single file, works on any static host instantly |

---

## UI

```
┌──────────────────────────────────────────────────────────────┐
│  • DarkDork                                       ◐ light   │
├──────────────────────────────────────────────────────────────┤
│                                                              │
│              Recon &                                         │
│              Dork Toolkit                                    │
│         AUTHORIZED SECURITY RESEARCH ONLY                    │
│                                                              │
│   ┌──────────────┐  ┌──────────────┐  ┌──────────────┐       │
│   │  01          │  │  02          │  │  03          │       │
│   │  Google      │  │  Bug Bounty  │  │  OSINT       │       │
│   │  Dorking     │  │  Search      │  │  Toolkit     │       │
│   │  dorks  ↗    │  │  recon  ↗   │  │  intel  ↗    │       │
│   └──────────────┘  └──────────────┘  └──────────────┘       │
│                                                              │
│         48 Dork Presets   60 BB Queries   20 OSINT Tools     │
│                                                              │
│  [3D particle globe rotates in background, reacts to mouse]  │
└──────────────────────────────────────────────────────────────┘
```

---

## Dork Categories

```
files    → open dirs, .env, .git, SSH keys, SQL dumps, Dockerfiles, Terraform, kubeconfig
creds    → AWS keys, GitHub tokens, Slack tokens, JWT secrets, API keys, RSA private keys
login    → WordPress, phpMyAdmin, cPanel, Jenkins, Kibana, Grafana, Elasticsearch
vulns    → SQL errors, PHP fatal errors, stack traces, Django debug, Laravel whoops, phpinfo
cloud    → S3 bucket listing, Azure blob public containers
iot      → live webcams, Hikvision cameras
osint    → email lists, CSV databases, VPN configs, Google Docs leaks
```

---

## Bug Bounty Recon Categories

```
recon      → directory listing, login pages, WordPress, subdomains, sub-subdomains, Pastebin, LinkedIn
files      → config files, database files, log files, backups, .htaccess, install files
vulns      → SQL errors, phpinfo, backdoors, open redirects, Apache Struts, GeoServer, SQL injection
login      → admin portals, Drupal, Joomla
docs       → exposed documents (PDF, DOCX, PPT, CSV)
external   → Shodan · Censys (×3) · crt.sh · GitHub · Wayback (×2) · ThreatCrowd · OpenBugBounty
           · Reddit · Yandex MIME · WordPress backup archive
```

---

## OSINT Tools Library

```
recon      → Shodan · Censys · GreyNoise · LeakIX · Wayback Machine · VirusTotal
ip & dns   → MXToolbox · DNSdumpster · ViewDNS.info · SecurityTrails
email      → Hunter.io · HaveIBeenPwned
username   → WhatsMyName
breach     → DeHashed
network    → Exploit-DB · NIST NVD
geo        → Google Maps
metadata   → ExifTool online · TinEye
darkweb    → DarkSearch
```

---

## How to Use

**1. Pick a module from the dashboard**

Click `01 Google Dorking`, `02 Bug Bounty Search`, or `03 OSINT Toolkit`.

**2. Set your target** *(optional for Google dorks)*

```
site: [ tesla.com ]
```

Type any domain. Every dork you select will automatically prepend `site:tesla.com`.

**3. Pick a dork preset**

Click any card from the grid. Use the category tabs or search box to filter. The query loads instantly into the preview box.

**4. Read the syntax-highlighted preview**

```
site:tesla.com  intitle:"index of"  ".env"
──────────────  ───────────────────  ──────
  gold               cyan             white
  (site)           (operator)        (value)
```

**5. Search or copy**

- `↗ Search Google` — opens Google with the exact query in a new tab
- `⎈ Copy Query` — copies the raw query string to clipboard
- External tool dorks change the button to `↗ Open shodan.io` etc.

---

## External Tool Dorks

Dorks tagged `ext` and `domain` in the Bug Bounty module open non-Google tools directly. A target domain is required.

| Dork | Opens |
|---|---|
| Find subdomains | Google — `site:*.target.com` |
| Certificate Transparency | `crt.sh/?q=%.target.com` |
| Search in Shodan | `shodan.io/search?query=target.com` |
| Search in Censys (×3) | `censys.io` — IPv4 / Domain / Certificates |
| Check in ThreatCrowd | `threatcrowd.org/domain.php?domain=...` |
| Search in Wayback (×2) | `web.archive.org` — URL and wildcard variants |
| Search in GitHub | `github.com/search?q=*.target.com` |
| LinkedIn Employees | Google — `site:linkedin.com employees target` |
| Pastebin Entries | Google — `site:pastebin.com target.com` |
| Search Reddit | `reddit.com/search/?q=target.com` |
| OpenBugBounty | `openbugbounty.org/search/?search=...` |
| WP Config Backup | Wayback Machine archive search |
| Yandex SWF MIME | `yandex.com` MIME-type SWF search |

---

## Run Locally

No build step required.

```bash
git clone https://github.com/0xcgz/0xcgz.github.io
cd 0xcgz.github.io
open index.html          # macOS
# or double-click index.html in your file manager
```

Or visit: **[0xcgz.github.io](https://0xcgz.github.io)**

---

## Project Structure

```
0xcgz.github.io/
├── index.html    ← entire app (HTML + CSS + JS, zero dependencies)
└── README.md     ← you are here
```

Everything lives in a single `index.html`. No npm, no webpack, no framework. Open and it works.

---

## What's New vs v1

- **3-in-1 dashboard** — dedicated modules for Dorking, Bug Bounty, and OSINT instead of one flat list
- **Bug Bounty module** — 60+ recon-specific queries with external tool launchers
- **Redesigned UI** — DM Sans + Space Mono typography, numbered cards, centered hero, stat counters
- **3D background** — interactive Fibonacci sphere particle network with mouse parallax and HVT node pulsing
- **Category tab system** — filter by type across all three modules
- **Improved dark mode** — warm near-black palette with proper depth layering, readable in both themes
- **No emojis** — clean typographic interface, no decorative icons
- **GitHub Pages safe** — zero external JS dependencies, fully self-contained single file

---

## Planned for Next Update

- Keyboard shortcuts (`Ctrl+K` domain focus, `/` filter, `Enter` search)
- Dork history — last 10 used queries persisted in localStorage
- Export mode — dump all dorks for a domain as `.txt` or `.md`
- Quick-copy on card — right-click a card to copy without selecting
- Custom dork builder — add your own presets, persisted in localStorage

---

## Ethical Use

> This tool is intended for **authorized security research**, **penetration testing on systems you own or have permission to test**, and **OSINT investigation within legal boundaries**.

- Do not use dorks to access systems without explicit written permission
- Unauthorized access to computer systems is illegal in most jurisdictions
- Google may temporarily rate-limit IPs performing rapid automated searches
- Some external tools require accounts or enforce their own rate limits

**This tool generates search queries only. It performs no hacking.**

---

## Contributing

Dork suggestions, tool additions, and bug fixes welcome.

1. Fork the repo
2. Edit the `DORKING_DATA`, `BUGBOUNTY_DATA`, or `OSINT_TOOLS` arrays in `index.html`
3. Open a pull request with a short description of what you added

---

## License

MIT — do whatever you want, just don't be evil.

---

<div align="center">

built by [0xcgz](https://0xcgz.github.io) · for the security community

</div>
