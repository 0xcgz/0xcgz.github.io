<div align="center">

```
██████╗  █████╗ ██████╗ ██╗  ██╗██████╗  ██████╗ ██████╗ ██╗  ██╗
██╔══██╗██╔══██╗██╔══██╗██║ ██╔╝██╔══██╗██╔═══██╗██╔══██╗██║ ██╔╝
██║  ██║███████║██████╔╝█████╔╝ ██║  ██║██║   ██║██████╔╝█████╔╝ 
██║  ██║██╔══██║██╔══██╗██╔═██╗ ██║  ██║██║   ██║██╔══██╗██╔═██╗ 
██████╔╝██║  ██║██║  ██║██║  ██╗██████╔╝╚██████╔╝██║  ██║██║  ██╗
╚═════╝ ╚═╝  ╚═╝╚═╝  ╚═╝╚═╝  ╚═╝╚═════╝  ╚═════╝ ╚═╝  ╚═╝╚═╝  ╚═╝
```

**Search Beyond the Surface.**

*Advanced OSINT, Google Dorking, and Bug Bounty reconnaissance in one unified toolkit.*

<br>

[![Live](https://img.shields.io/badge/live-0xcgz.github.io-e85535?style=flat-square&logo=github&logoColor=white)](https://0xcgz.github.io)
[![License](https://img.shields.io/badge/license-MIT-111111?style=flat-square)](LICENSE)
[![Dorks](https://img.shields.io/badge/dork_presets-100%2B-e0ac3a?style=flat-square)](#01--google-dorking)
[![BB Queries](https://img.shields.io/badge/bb_queries-60%2B-6aaccc?style=flat-square)](#02--bug-bounty-search)
[![OSINT Tools](https://img.shields.io/badge/osint_tools-200%2B-4aaa6a?style=flat-square)](#03--osint-toolkit)
[![Zero Deps](https://img.shields.io/badge/dependencies-zero-111111?style=flat-square)](#run-locally)

</div>

---

## What is DarkDork?

**DarkDork** is a browser-based recon toolkit — no backend, no login, no tracking. Open the file and start hunting.

Three modules live in a single zero-dependency HTML file: a Google Dork builder with live syntax highlighting, a Bug Bounty recon suite with external tool launchers, and a radial OSINT mindmap with 200+ curated tools across 12 categories. Set a target domain once and every query auto-injects `site:` for you.

---

## Modules

### 01 — Google Dorking

100+ hand-picked search operators to surface exposed files, admin panels, login pages, and sensitive data indexed by Google. Live query preview with operator colour-coding before you search.

### 02 — Bug Bounty Search

60+ recon queries targeting common bug bounty surfaces — exposed configs, login panels, vuln signatures, WordPress installs. Direct launchers for Shodan, crt.sh, Wayback Machine, Censys, GitHub, ThreatCrowd, and more.

### 03 — OSINT Toolkit

200+ intelligence tools mapped across 12 categories — from WHOIS and DNS to social, dark web, and threat intel — in an interactive radial mindmap. Drag, zoom, search, and click to open any tool. Tag filters surface free / registration-required / local tools instantly.

---

## Features

| | Feature | Description |
|---|---|---|
| `◉` | **3D Recon Globe** | 250-node Fibonacci sphere, mouse parallax, pulsing HVT nodes |
| `◎` | **Live Query Preview** | Syntax-highlighted preview — operators in cyan, values in white, site in gold |
| `⊞` | **OSINT Radial Map** | Drag-to-pan, scroll-to-zoom, momentum physics, search-and-fly-to |
| `⌦` | **Target Domain Injection** | Set a domain once — auto-injects `site:` into every dork |
| `⏱` | **Query History** | Every search and copy logged per session, re-runnable in one click |
| `⊕` | **Custom Dork Builder** | Chain operators token by token, search or copy the full assembled query |
| `⬇` | **Export** | Download current tab's dorks as `.txt` — pipe into your scripts |
| `⎈` | **Per-Card Copy** | Copy any query without selecting it first |
| `⌘K` | **Command Palette** | Fuzzy-search across all dorks, tools, and navigation actions |
| `◐` | **Dark / Light Mode** | Clean toggle, preference saved to localStorage |
| `∅` | **Zero Dependencies** | Pure HTML/CSS/JS — no npm, no build step, no framework |

---

## UI

```
┌──────────────────────────────────────────────────────────────────┐
│  DarkDork   ← back        ⬇ export   ⏱ history   ? help   ◐ light│
├──────────────────────────────────────────────────────────────────┤
│                                                                  │
│              Search Beyond the Surface.                          │
│   Advanced OSINT, Google Dorking, and Bug Bounty recon           │
│              in one unified toolkit.                             │
│                                                                  │
│  ┌────────────────┐  ┌────────────────┐  ┌────────────────┐      │
│  │  01            │  │  02            │  │  03            │      │
│  │  Google        │  │  Bug Bounty    │  │  OSINT         │      │
│  │  Dorking       │  │  Search        │  │  Toolkit       │      │
│  │                │  │                │  │                │      │
│  │  100+ presets  │  │  recon + ext   │  │  200+ tools    │      │
│  │  dorks  ↗      │  │  recon  ↗      │  │  intel  ↗      │      │
│  └────────────────┘  └────────────────┘  └────────────────┘      │
│                                                                  │
│    100+ Dork Presets     60+ BB Queries     200+ OSINT Tools      │
│                                                                  │
│   [ 3D particle globe — rotates, reacts to mouse movement ]      │
└──────────────────────────────────────────────────────────────────┘
```

---

## Dork Categories

```
files    →  open dirs · .env · .git config · SSH keys · SQL dumps
            Dockerfiles · Terraform state · kubeconfig · backup archives

creds    →  AWS access keys · GitHub personal tokens · Slack bot tokens
            JWT secrets · API keys in .env · RSA private keys

login    →  WordPress admin · phpMyAdmin · cPanel · Jenkins CI
            Kibana · Grafana · Elasticsearch

vulns    →  MySQL errors · PHP fatal errors · stack traces exposed
            Django debug mode · Laravel whoops · phpinfo()

cloud    →  S3 bucket listing · Azure blob public containers

iot      →  live webcams · Hikvision cameras

osint    →  email lists · customer CSV databases · VPN configs · Google Docs leaks
```

---

## Bug Bounty Recon Categories

```
recon      →  directory listing · login pages · WordPress · subdomains
               sub-subdomains · Pastebin entries · LinkedIn employees

files      →  config files · database files · log files · backups
               .htaccess · install/setup files

vulns      →  SQL errors · phpinfo · backdoors · open redirects
               Apache Struts RCE · GeoServer · SQL file injection

login      →  admin portals · Drupal · Joomla database

docs       →  exposed PDFs · DOCX · PPT · CSV documents

external   →  Shodan · Censys ×3 · crt.sh · GitHub · Wayback ×2
               ThreatCrowd · OpenBugBounty · Reddit · Yandex MIME
               WordPress backup archive
```

---

## OSINT Toolkit — 12 Categories

```
Username        →  WhatsMyName · Sherlock · Namechk · KnowEm · Spokeo · Pipl
                   Social-Analyzer · IDCrawl · TruePeopleSearch · WebMii

Email Address   →  Hunter.io · Epieos · Phonebook.cz · EmailRep.io · HaveIBeenPwned
                   DeHashed · LeakCheck · Snusbase · BreachDirectory · IntelligenceX
                   MXToolbox header analyzer

Domain / IP     →  MXToolbox · DNSdumpster · SecurityTrails · ViewDNS.info · IPinfo.io
                   AbuseIPDB · Pulsedive · Criminal IP · GreyNoise · OTX AlienVault
                   crt.sh · Censys · ARIN Whois · DomainTools

Search Engines  →  Shodan · Censys · FOFA · ZoomEye · BinaryEdge · Netlas
                   grep.app · PublicWWW · GitHub Code Search · Searchcode
                   Ahmia · DarkSearch · IntelligenceX TOR · OnionSearch

Images / Video  →  TinEye · Google Images · Yandex Images · Bing Visual Search
                   PimEyes · FaceCheck.ID · ExifTool · Forensically · FotoForensics
                   InVID WeVerify · YouTube DataViewer

Social Networks →  Twitter Advanced Search · Followerwonk · Twint
                   StalkFace · Picuki · Osintgram · LinkedIn Search
                   RedditMetis · TGstat · Exolyt

Geolocation     →  Google Maps · Yandex Maps · Sentinel Hub · Mapillary
                   SunCalc · PeakVisor · FlightAware · Flightradar24
                   MarineTraffic · VesselFinder · WiGLE

Archives        →  Wayback Machine · Archive.today · TimeTravel · DocumentCloud

Phone Numbers   →  Truecaller · NumVerify · Thatsthem · FreeCarrierLookup · HLR Lookup

Dark Web        →  Ahmia · DarkSearch · OnionLand Search · Tor66 · Dark.fail
                   IntelligenceX TOR · PSBDMP · LeakIX · Onyphe

Threat Intel    →  NIST NVD · CVE Mitre · Exploit-DB · Sploitus · Vulners
                   AttackerKB · VirusTotal · MalwareBazaar · Hybrid Analysis
                   URLScan.io · ThreatCrowd · IBM X-Force · OpenCTI

Images · Video  →  (see above)
```

---

## How to Use

**1. Pick a module from the dashboard**

Click `01 Google Dorking`, `02 Bug Bounty Search`, or `03 OSINT Toolkit`. Or use keyboard shortcuts.

**2. Set your target** *(Dorking + Bug Bounty)*

```
site: [ tesla.com ]
```

Set it once. Every dork auto-prepends `site:tesla.com`. Carries over between modules.

**3. Select a preset**

Click any card. Use the category tabs or the search box to filter. The query renders instantly.

**4. Read the preview**

```
site:tesla.com  intitle:"index of"  ".env"
──────────────  ───────────────────  ──────
    gold              cyan            white
   (site)           (operator)       (value)
```

**5. Search or copy**

- `↗ Search Google` — opens the exact query in a new tab
- `⎈ Copy Query` — copies raw string to clipboard
- External dorks become `↗ Open shodan.io`, `↗ Open crt.sh`, etc.

**6. OSINT Map**

- **Drag** to pan · **Scroll** to zoom · **Click a node** to open the tool or expand a branch
- **Search** in the header to fly to any tool
- **Tag filters** — `Free only` · `[R] Registration` · `[T] Local tool` · `[D] Dork`
- **⊙ Reset** to return to centre · **⊞ Labels** to cycle label density

---

## Keyboard Shortcuts

| Key | Action |
|---|---|
| `G` | Google Dorking |
| `B` | Bug Bounty |
| `O` | OSINT Map |
| `H` | Toggle history panel |
| `/` | Focus search / filter |
| `Esc` | Back / close |
| `⌘K` / `Ctrl+K` | Command palette |
| `↑ ↓ Enter` | Navigate command palette |

---

## External Tool Launchers

Dorks tagged `ext` + `domain` in Bug Bounty open external tools directly. Target domain required.

| Dork | Destination |
|---|---|
| Find subdomains | Google — `site:*.target.com` |
| Certificate Transparency | `crt.sh/?q=%.target.com` |
| Shodan | `shodan.io/search?query=target.com` |
| Censys IPv4 / Domain / Certs | `censys.io` — three separate searches |
| ThreatCrowd | `threatcrowd.org/domain.php?domain=...` |
| Wayback Machine ×2 | URL archive + wildcard variant |
| GitHub Code Search | `github.com/search?q=*.target.com` |
| LinkedIn Employees | Google — `site:linkedin.com employees target` |
| Pastebin | Google — `site:pastebin.com target.com` |
| Reddit | `reddit.com/search/?q=target.com` |
| OpenBugBounty | `openbugbounty.org/search/?search=...` |

---

## Run Locally

```bash
git clone https://github.com/0xcgz/0xcgz.github.io
cd 0xcgz.github.io
open index.html        # macOS
# or just double-click index.html
```

Or use it live: **[0xcgz.github.io](https://0xcgz.github.io)**

---

## Project Structure

```
0xcgz.github.io/
├── index.html   ←  entire app — HTML + CSS + JS, zero dependencies
└── README.md    ←  you are here
```

One file. No npm. No webpack. No framework. Open and it works.

---

## Ethical Use

> Intended for **authorized security research**, **penetration testing on systems you own or have explicit permission to test**, and **OSINT investigation within legal boundaries**.

- Do not use dorks to access systems without written permission
- Unauthorized access is illegal in most jurisdictions
- Google may rate-limit IPs performing rapid searches
- Some external tools require accounts or enforce rate limits

**This tool generates search queries only. It performs no exploitation.**

---

## Contributing

Dork suggestions, tool additions, and bug reports welcome.

1. Fork the repo
2. Edit `DORKING_DATA`, `BUGBOUNTY_DATA`, or `OSINT_TREE` in `index.html`
3. Open a pull request with a short description of what you added

---

## License

MIT — do whatever you want, just don't be evil.

---

<div align="center">

© 2026 [0xcgz](https://0xcgz.github.io) · built for the security community

</div>
