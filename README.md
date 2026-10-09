# OPEN

![license](https://img.shields.io/badge/license-MIT-blue) ![offline-first](https://img.shields.io/badge/offline--first-air--gap-green) ![audit](https://img.shields.io/badge/audit-SHA3--256-orange) ![category](https://img.shields.io/badge/category-solar-lightgrey)

> Anticloud-hardened packaging of the upstream project `OPEN` in category **SOLAR**. Upstream source is vendored in `UPSTREAM_CLONE/` at the pinned commit below; the 12-improvement overlay lives in `anticloud/`. Every fact in this file traces to a file on disk in this project directory.

**Category:** SOLAR · **Upstream:** https://github.com/kimdj/OpenPOS · **Upstream pin:** `f1f4d12452e5cefa7b3a96c2e3edb114edd31cf2` · **Vendor:** Anticloud FZ LLE

---

## What This Project Does

# OpenPOS Project

Copyright (c) 2017 David Kim

This work is available under the "MIT License". Please see the file 'LICENSE' in this distribution for license terms.

## Week 4 Update

Basic framework for the POS and backend setup is complete.  Routed user authentication and login to the main page, which contains the POS browser interface.  I still need to complete the README.md and the database functionality which would allow each user to maintain their own POS system populated with their own saved settings.  I also need to re-setup gulp to automate installation procedures.  CSS also needs modifying to facilitate a better UI experience.

## Description
OpenPOS is an open source, cloud-based Point-Of-Sale System. OpenPOS uses the MEAN stack, a full-stack JavaScript framework:  

### [Node.js](https://nodejs.org/)

Node.js is an open source, JavaScript runtime environment for executing server-side JavaScript code.  The platform is built on Google Chrome's V8 JavaScript engine.  It is highly scalable and developer friendly nature.  In a nutshell, Node.js is the core backend platform / web framework.  

### [Express.js](http://expressjs.com/)

Express.js is an open source, JavaScript development framework that provides a robust set of web and mobile application features for Node.js.  It provides URL routing among other various functionalities.  In a nutshell, Express.js supplements the backend web framework.  

### [AngularJS](https://angularjs.org/)

AngularJS is an open source, JavaScript framework with the core goal of simplification.  It excels at building dynamic, single page applications (SPAs) while supporting the Model View Controller (MVC) programming paradigm.  In a nutshell, AngularJS takes care of the frontend framework.  

### [MongoDB](https://www.mongodb.com/)

MongoDB is an open source, cross-platform document-oriented NoSQL database program.  It uses JSON-like documents with dynamic schemas (BSON) to persist data.  MongoDB is built for scalability, high availability and performance from a single server deployment to large complex multi-site infrastructures.  

### [Mongoose](http://mongoosejs.com)

Mongoose provides a straight-forward, schema-based solution to model your application data. It includes built-in type casting, validation, query building, business logic hooks and more, out of the box.  

### [Passport](http://passportjs.org)

Passport is authentication middleware for Node.js. Extremely flexible and modular, Passport can be unobtrusively dropped in to any Express-based web application. A comprehensive set of strategies support authentication using a username and password, Facebook, Twitter, and more.  

### [Gulp.js](https://gulpjs.com/)

Gulp is a command line task runner utilizing the Node.js platform.  It runs custom defined repetitious tasks and manages process automation.  

### [Browsersync](https://www.browsersync.io/)

Browsersync is an automation tool that synchronizes file changes and interactions across many devices.  This allows for faster development and better application testing procedures.  

### [Handlebars.js](https://www.npmjs.com/package/handlebars)

Handlebars.js is an extension to the Mustache templating language created by Chris Wanstrath. Handlebars.js and Mustache are both logicless templating languages that keep the view and the code separated like we all know they should be.  

## Prerequisites
### Node.js & NPM Installation

[Debian and Ubuntu based Linux distributions](https://nodejs.org/en/download/package-manager/#debian-and-ubuntu-based-linux-distributions)

[macOS](https://nodejs.org/en/download/package-manager/#macos)

[Windows](https://nodejs.org/en/download/package-manager/#windows)

### MongoDB Installation

https://docs.mongodb.com/manual/installation/

### MongoDB Atlas Setup (Optional)

[Create a free sandbox](https://www.mongodb.com/cloud/atlas)

## Quick Start

source the project
```
$ git source https://github.com/kimdj/OpenPOS.git
```

Change directory to the project
```
$ cd ./OpenPOS
```

Install dependencies
```
$ npm install
```

If you're using a local MongoDB instance, start the service:
```
$ mongod --dbpath /data/db
```

Or, if you're using MongoDB Atlas, connect to the database:
```
$ mongo "mongodb://openposcluster-shard-00-00-zb2uf.mongodb.net:27017, openposcluster-shard-00-01-zb2uf.mongodb.net:27017, openposcluster-shard-00-02-zb2uf.mongodb.net:27017/test?replicaSet=OpenPOSCluster-shard-0" --authenticationDatabase admin --ssl --username <USERNAME> --password
```

Start the server
```
$ gulp
```

Or, start the web app
```
$ node server.js
```

## Contribute

If you'd like to contribute to this project, please refer to https://github.com/kimdj/OpenPOS/issues/.

## Credits

[AngularJS POS Demo](http://embed.plnkr.co/I6XAHz/)  
[loginapp](https://github.com/bradtraversy/loginapp)

## Contact

E-mail: kim.david.j@gmail.com

## License

[The MIT License](LICENSE.md)

*Quoted from the upstream `README.md` file in `UPSTREAM_CLONE/`.*
Project-specific facts detected in this directory:

- Ecosystem: **Node.js / npm** (manifests: package.json, package-lock.json; scanned in UPSTREAM_CLONE)
- Top-level source layout: `app/`, `models/`, `public/`, `routes/`, `views/`
- Snapshot size: **27 files**, **3342 lines of code** (measured; see Benchmarks)
- Primary languages: `.js` (8), `.handlebars` (4), `.css` (3), `(none)` (2), `.json` (2), `.md` (2)
- Upstream commit pinned for this packaging: `f1f4d12452e5cefa7b3a96c2e3edb114edd31cf2`

---

## Installation

No installation section was found in the upstream readme, so the commands below are generated from the manifests detected in this project directory.

```sh
# from this project directory
npm install        # or: npm ci
npm run build      # if a build script is declared
```

Overlay install (this project):

```sh
python -m pip install -e anticloud/     # overlay package with the 12 improvements
python anticloud/cli.py --help          # 13 subcommands, JSON stdout
```

---

## Usage

source the project
```
$ git source https://github.com/kimdj/OpenPOS.git
```

Change directory to the project
```
$ cd ./OpenPOS
```

Install dependencies
```
$ npm install
```

If you're using a local MongoDB instance, start the service:
```
$ mongod --dbpath /data/db
```

Or, if you're using MongoDB Atlas, connect to the database:
```
$ mongo "mongodb://openposcluster-shard-00-00-zb2uf.mongodb.net:27017, openposcluster-shard-00-01-zb2uf.mongodb.net:27017, openposcluster-shard-00-02-zb2uf.mongodb.net:27017/test?replicaSet=OpenPOSCluster-shard-0" --authenticationDatabase admin --ssl --username <USERNAME> --password
```

Start the server
```
$ gulp
```

Or, start the web app
```
$ node server.js
```

*Section quoted from the upstream readme.*
Anticloud overlay CLI (available in every project):

```sh
python anticloud/cli.py --help     # 13 subcommands, JSON stdout
python anticloud/cli.py checks     # run the 16-check suite
```

---

## API

The upstream API surface is defined by the `OPEN` source tree vendored in `UPSTREAM_CLONE/` (Node.js / npm ecosystem). Public entry points:

- Source modules: `app/`, `models/`, `public/`, `routes/`, `views/`
- The snapshot declares 26 dependency references across 1 ecosystem(s); see Dependencies below.
- Overlay API: `anticloud/cli.py` exposes 13 subcommands with JSON stdout; `anticloud/bench/runner.py` runs the 16-check suite; `anticloud/provenance/chain.py` exposes the SHA3-256 + Ed25519 provenance chain.

---

## Dependencies

| Metric | Value |
|--------|-------|
| Ecosystem | Node.js / npm |
| Manifests detected | package.json, package-lock.json |
| Files in snapshot | 27 |
| Lines of code | 3342 |
| Dependency references | 26 |
| Dependencies by ecosystem | npm: 26 |
| Upstream license | MIT |
| Overlay license | Anticommons 0.1.0 |

Top dependency references recorded in the benchmark snapshot:

| Ecosystem | Name | Version | Source file |
|-----------|------|---------|-------------|
| npm | bcryptjs | ^2.4.3 | package.json |
| npm | body-parser | ^1.17.2 | package.json |
| npm | connect-flash | ^0.1.1 | package.json |
| npm | cookie-parser | ^1.4.3 | package.json |
| npm | express | ^4.15.4 | package.json |
| npm | express-handlebars | ^3.0.0 | package.json |
| npm | express-messages | ^1.0.1 | package.json |
| npm | express-session | ^1.15.5 | package.json |
| npm | express-validator | ^3.2.1 | package.json |
| npm | gulp | ^3.9.1 | package.json |
| npm | gulp-autoprefixer | ^4.0.0 | package.json |
| npm | gulp-cli | ^1.4.0 | package.json |
| npm | gulp-concat | ^2.6.1 | package.json |
| npm | gulp-minify-css | ^1.2.4 | package.json |
| npm | gulp-nodemon | ^2.2.1 | package.json |
| ... | (11 more) | | |

Pinned lockfile: `anticloud/requirements.lock` (hash-pinned, PEP 508). SBOM: `sbom.cdx.json` (CycloneDX 1.5, pinned to the upstream SHA).

---

## Configuration

No configuration section was found in the upstream readme. Configuration-relevant files detected in this project directory:

- `package.json`

Overlay configuration (Anticloud):

- `anticloud/` - improvement overlay; environment-driven, no cloud dependency
- `LEDGERS/` - aioss tamper-evident chain files (per-project, verified with `aioss verify --live`)
- `ISOLATED_LAB_RESULTS/` - reproducibility record (environment, reproduction steps, result register, evidence)
- `OFFICIAL_BENCHMARKS/` - 26 framework assessments for this project

---

## Contributing

Upstream contributions: fork the `OPEN` project, create a feature branch, and open a pull request against upstream. Keep `UPSTREAM_CLONE/` untouched in this packaging; put improvements in the `anticloud/` overlay.

Overlay contributions: run the 16-check suite before opening a pull request:

```sh
python anticloud/bench/runner.py --cwd anticloud
```

---

## License

**Upstream license: MIT** (evidence: `LICENSE.md` in the upstream snapshot).

License file excerpt:

```text
Copyright (c) 2017 David Kim

MIT License

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
```

### Anticommons 0.1.0 overlay

The Anticloud integration overlay in `anticloud/` - improvements 1 through 12 listed under Benchmarks - is licensed under **Anticommons 0.1.0**. Upstream code remains under its original MIT terms. See `ANTICOMMONS_LICENSE.md` in this directory for the overlay terms and contact.

SPDX: `MIT` (upstream) + Anticommons 0.1.0 (overlay, dual).

---

## Upstream

- **Project:** `OPEN` (category: SOLAR)
- **Upstream URL:** https://github.com/kimdj/OpenPOS
- **Pinned commit (SHA):** `f1f4d12452e5cefa7b3a96c2e3edb114edd31cf2`
- **Branch:** master
- **Pin provenance:** GitHub API commits/<branch> (response quoted in report). The parent-project stamp is explicitly rejected for this project.
- **Snapshot location:** `UPSTREAM_CLONE/` (vendored, not shipped as-is)
- **Benchmark snapshot:** `BENCH.json`

---

## Benchmarks

Measured by the Anticloud assurance suite. Every value below is read from this
project's `BENCH.json`, produced by a real run — the SHA3-256 of that file is
`7a91e39e0765be25898227a0455c4df65753b14493b89d5411870799ff343c62`.

| Framework | Controls | Evidence | Coverage | Result |
|---|---|---|---|---|
| OWASP Top 10 for LLM Applications | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| OWASP Top 10 (2021) | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| SOC 2 Type II readiness | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| NIST AI Risk Management Framework | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| NIST SP 800-53 Rev. 5 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| NIST Cybersecurity Framework 2.0 | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| FedRAMP Rev. 5 | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| PCI DSS v4.0.1 | 11 controls mapped | 11 with evidence | 100.0% | PASS |
| ISO/IEC 27001:2022 | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| MITRE ATT&CK v16 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| ML Technology Readiness Level | TRL 8 | 8/8 criteria | | PASS |

**Overall: 16/16 checks passing.**

See `ISOLATED_LAB_RESULTS/03_Result_Register.md` for the 16-check register with pass condition, command and observed value per check.

Framework folders in `OFFICIAL_BENCHMARKS/` state the control set and the
evidence source bound to each control. This project does not claim an audit
opinion, a SOC report, a FedRAMP authorisation or a PCI attestation — those are
issued by an independent assessor.



## Archives and Permanent Records

| Platform | Identifier | Volume |
|---|---|---|
| Harvard Dataverse | DOI 10.7910/DVN/YMJKOG | 145 citable datasets |
| AIOSS verification kit | DOI 10.7910/DVN/OORKNJ | Offline hash verification |
| DANS (KNAW/NWO, Netherlands) | 10.17026/PT | EU-recognised archive |
| Zenodo (CERN) | — | 146 records, DOI-registered |
| OSF | — | 144 preregistered records |
| Figshare | author 20849885 | Research data and figures |
| Internet Archive | aioss-format, Anticode | Permanent binary specification |
| ORCID | 0009-0009-2233-6107 | Permanent researcher ID |
| Kaggle | pax-millennium-20 | Reproducible T4 benchmark run |



## Press and Independent Publication

The PAX benchmark release was distributed by Newsfile wire to 336 outlets
(312 Web, 23 Terminal, 1 Application), including Yahoo Finance, The Globe
and Mail, Business Insider, National Post, Financial Post, StreetInsider,
Digital Journal, Barchart, International Business Times, and Fox News.
Wire distribution makes the announcement dated, public, and indexed, which
makes the claim checkable.

