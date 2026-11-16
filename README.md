# SpiderFoot Cookbook

<!-- ZQM-START -->
<!-- markdownlint-disable MD033 -->
<p align="center">
  <strong>ZQM Computing — Geospatial Engineering & Scientific Computing</strong><br>
  <a href="https://github.com/ZQM-Computing">ZQM Computing</a>
</p>
<!-- markdownlint-enable MD033 -->
<!-- ZQM-END -->

![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)

A **SpiderFoot cookbook** for passive OSINT automation as a service. Patterns are drawn from the ZQM fleet's SpiderFoot 4.0.0 installs as Windows services on port 5001 with tailnet-plus-LAN-only firewall rules. Passive use only; no scan is run in this cookbook, and no API keys are stored in it. It is intended for OSINT practitioners who automate passive collection behind a private service. Validate each pattern against your own data, software versions, and operating environment before adopting it.

## Repository role and status

**Status:** Active, public — seeding. Pattern passes land in follow-up work from fleet-verified setups; the tables below list what is planned, not what is already written.

**What this repository is:** SpiderFoot patterns — see the table below.

**What it contributes:** Part of the ZQM Computing geospatial portfolio. The umbrella index for the series is [geospatial-cookbooks](https://github.com/ZQM-Computing/geospatial-cookbooks).

**Standing:** This repository is maintained independently. Automated checks cover only the paths and environments configured in its workflows; they do not establish production readiness or operational certification.

## Who this is for

OSINT practitioners who automate passive collection behind a private service.

## Prerequisites

- SpiderFoot 4.0.0
- A service host (Windows service pattern as on the fleet)
- Module API keys, kept out of repos, for the modules that need them

## Patterns (planned)

| # | Example | What it will demonstrate |
|---|---------|--------------------------|
| 01 | `01-service-deploy` | Deploying SpiderFoot as a service with a private-only firewall scope |
| 02 | `02-passive-scan-config` | Configuring passive-only scans and module selection |
| 03 | `03-module-keys` | Where module keys live and how they stay out of version control |

## Repository layout

```text
spiderfoot-cookbook/
├── examples/          # pattern passes, landing in follow-up work
├── README.md
└── LICENSE
```

## Roadmap

- First pattern pass: the first two table rows
- Second pass: the remaining rows, from fleet-verified setups

## Contributing

A contributing guide lands with the first pattern pass. Report security issues to <zqmcomputing@gmail.com> — please do not open a public issue for those.

## More from this series

- [theharvester-cookbook](https://github.com/ZQM-Computing/theharvester-cookbook) — Passive reconnaissance: domains, emails, and hosts from public sources
- [amass-cookbook](https://github.com/ZQM-Computing/amass-cookbook) — Passive subdomain enumeration and graph output
- [shodan-cookbook](https://github.com/ZQM-Computing/shodan-cookbook) — Internet-device search from the command line
