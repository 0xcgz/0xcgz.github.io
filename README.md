<div align="center">

```
██████╗  █████╗ ██████╗ ██╗  ██╗██████╗  ██████╗ ██████╗ ██╗  ██╗
██╔══██╗██╔══██╗██╔══██╗██║ ██╔╝██╔══██╗██╔═══██╗██╔══██╗██║ ██╔╝
██║  ██║███████║██████╔╝█████╔╝ ██║  ██║██║   ██║██████╔╝█████╔╝ 
██║  ██║██╔══██║██╔══██╗██╔═██╗ ██║  ██║██║   ██║██╔══██╗██╔═██╗ 
██████╔╝██║  ██║██║  ██║██║  ██╗██████╔╝╚██████╔╝██║  ██║██║  ██╗
╚═════╝ ╚═╝  ╚═╝╚═╝  ╚═╝╚═╝  ╚═╝╚═════╝  ╚═════╝ ╚═╝  ╚═╝╚═╝  ╚═╝
```

**Google Dork Query Builder · OSINT Tool Library · Recon Automation**

[![Live](https://img.shields.io/badge/live-0xcgz.github.io-111111?style=flat-square&logo=github)](https://0xcgz.github.io)
[![License](https://img.shields.io/badge/license-MIT-111111?style=flat-square)](LICENSE)
[![Dorks](https://img.shields.io/badge/dorks-300%2B-111111?style=flat-square)](https://0xcgz.github.io)
[![Tools](https://img.shields.io/badge/osint%20tools-100%2B-111111?style=flat-square)](https://0xcgz.github.io)
[![Made with](https://img.shields.io/badge/built%20with-vanilla%20html-111111?style=flat-square)](https://0xcgz.github.io)

</div>

---

## What is DarkDork?

**DarkDork** is a browser-based Google Dork builder and OSINT toolkit. No backend, no login, no tracking — just open it and start dorking.

You pick a target domain, select a dork preset, and see the full query rendered live before you search. It also ships with a curated library of 100+ external OSINT tools organized into searchable categories.

---

## Features

| Feature | Description |
|---|---|
| 🎯 **Target Domain Input** | Set a domain once — it auto-injects `site:` into every query |
| ⚡ **Live Query Preview** | Syntax-highlighted preview before you hit search |
| ★ **Top Dorks** | Pinned section of the 12 most-used dorks |
| 🗂 **300+ Dork Presets** | Categorized: files, creds, login, vulns, iot, docs, cloud, osint, recon |
| 🌐 **External Tool Dorks** | Opens Shodan, crt.sh, Wayback, Censys, GitHub and more directly |
| ⬡ **OSINT Tools Library** | 100+ tools across 10 categories with one-click launch |
| 🔍 **Live Search Filter** | Filter any dork by name, query string, or category |
| ◑ **Dark Mode** | Toggles cleanly, preference saved to localStorage |
| 📋 **Copy to Clipboard** | One click copies the full query |
| 🚫 **Zero Dependencies** | Pure HTML/CSS/JS — no npm, no build step, no framework |

---

## Screenshots

> *Light mode — dork builder with live query preview*

```
┌─────────────────────────────────────────────────────────┐
│  DarkDork                  google dork library  ◑ dark │
├─────────────────────────────────────────────────────────┤
│  site:  [ example.com                              ] ×  │
│                                                         │
│  ┌─────────────────────────────────────────────────┐    │
│  │ site:example.com intitle:"index of /" ".env"    │    │
│  └─────────────────────────────────────────────────┘    │
│  [↗ search google]  [⎘ copy]  [× clear]                │
│                                                         │
│  ★ top dorks — most used                               │
│  ┌──────────────┐ ┌──────────────┐ ┌──────────────┐     │
│  │ Open dirs    │ │ Exposed .env │ │ Admin panels │     │
│  │ intitle:...  │ │ intitle:...  │ │ inurl:admin  │     │
│  └──────────────┘ └──────────────┘ └──────────────┘     │
└─────────────────────────────────────────────────────────┘
```

---

## Dork Categories

```
files    → open dirs, .env, .git, SSH keys, SQL dumps, Dockerfiles, Terraform, YAML secrets
creds    → AWS keys, Stripe, GitHub tokens, Slack, Firebase, JWT, OAuth, 40+ API providers
login    → WordPress, phpMyAdmin, Joomla, Django, Jenkins, Grafana, Kibana, Jupyter, 30+ panels
vulns    → SQL errors, PHP errors, stack traces, debug pages, actuators, phpinfo, IIS, Nginx
iot      → webcams, Hikvision, SCADA, HMI, Mikrotik, QNAP, Ubiquiti, Modbus, Home Assistant
docs     → payroll sheets, NDAs, pentest reports, org charts, board minutes, pitch decks
cloud    → S3, Azure blobs, GCP, Firebase, Heroku, Vercel, Netlify, Cloudflare Workers
osint    → email lists, phone lists, Pastebin dumps, Trello, Notion, Airtable, Confluence leaks
recon    → 64 domain-targeted dorks + external tools (Shodan, crt.sh, Wayback, Censys, Reddit)
```

---

## OSINT Tools Library

Over **100 tools** organized into clickable categories. Each card opens the tool directly.

```
recon      → Shodan · Censys · FOFA · ZoomEye · GreyNoise · LeakIX · URLScan · VirusTotal
ip & dns   → DNSdumpster · SecurityTrails · IPinfo · AbuseIPDB · BGP.he.net · PassiveDNS
email      → Hunter.io · HaveIBeenPwned · EmailRep · Phonebook.cz · Snov.io · VoilaNorbert
username   → WhatsMyName · Sherlock · Namechk · KnowEm · IDCrawl · Spokeo · Pipl
breach     → DeHashed · LeakCheck · Snusbase · BreachDirectory · PSBDMP · GhostProject
network    → Exploit-DB · NVD · Vulners · Sploitus · OTX AlienVault · MalwareBazaar
geo        → SunCalc · Sentinel Hub · FlightAware · MarineTraffic · Mapillary · Overpass
metadata   → ExifTool · Forensically · FotoForensics · TinEye · PimEyes · Yandex Images
darkweb    → Ahmia · DarkSearch · IntelligenceX · Maltego · Dark.fail · Hunchly
```

---

## How to Use

**1. Set your target** *(optional)*

```
site: [ tesla.com ]
```

Type any domain. Every dork you select will automatically prepend `site:tesla.com` to the query.

**2. Pick a dork**

Click any card from the Top Dorks section or browse by category. The query loads instantly into the preview box.

**3. Read the preview**

```
site:tesla.com  intitle:"index of"  ".env"
──────────────  ─────────────────── ──────
  orange            teal              white
  (site)           (operator)        (value)
```

**4. Search or copy**

- `↗ search google` — opens Google with the exact query
- `⎘ copy` — copies the raw query string to clipboard
- External tools (Shodan, crt.sh, etc.) change the button to `↗ open shodan.io`

---

## External Tool Dorks

Some dorks in the `recon` category open non-Google tools. These are tagged `↗ ext` and require a domain.

| Dork | Opens |
|---|---|
| Find subdomains | `google.com` — `site:*.target.com` |
| Certificate Transparency | `crt.sh/?q=%.target.com` |
| Search in Shodan | `shodan.io/search?query=target.com` |
| Search in Censys (×3) | `censys.io` IPv4 / Domain / Certificates |
| Check in ThreatCrowd | `threatcrowd.org/domain.php?domain=...` |
| Search in Wayback | `web.archive.org` (×2 variants) |
| Search in GitHub | `github.com/search?q=*.target.com` |
| LinkedIn Employees | Google — `site:linkedin.com employees target` |
| Pastebin Entries | Google — `site:pastebin.com target.com` |
| Search Reddit | `reddit.com/search/?q=target.com` |
| OpenBugBounty | `openbugbounty.org/search/?search=...` |

---

## Run Locally

No build step required.

```bash
git clone https://github.com/0xcgz/0xcgz.github.io
cd 0xcgz.github.io
open index.html          # macOS
# or just double-click index.html in your file manager
```

Or just visit: **[0xcgz.github.io](https://0xcgz.github.io)**

---

## Project Structure

```
0xcgz.github.io/
└── index.html        ← entire app (HTML + CSS + JS, zero dependencies)
└── README.md         ← you are here
```

Everything lives in a single `index.html` file. No npm, no webpack, no framework. Open and it works.

---

## Ethical Use

> ⚠️ This tool is intended for **authorized security research**, **penetration testing on systems you own**, and **OSINT investigation within legal boundaries**.

- Do not use dorks to access systems without explicit permission
- Unauthorized access to computer systems is illegal in most jurisdictions
- Google may temporarily block IPs that perform rapid automated searches
- Some external tools require accounts or have rate limits

**This tool generates search queries only. It performs no hacking.**

---

## Contributing

Dork suggestions, tool additions, and bug fixes are welcome.

1. Fork the repo
2. Edit the `PRESETS` or `TOOLS` array in `index.html`
3. Open a pull request with a short description

---

## License

MIT — do whatever you want, just don't be evil.

---

<div align="center">

built by [0xcgz](https://0xcgz.github.io) · for the security community

</div>
