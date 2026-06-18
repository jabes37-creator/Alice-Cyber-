# Alice Cyber Community Edition

**Alice Cyber Community Edition** is an open-source defensive cybersecurity toolkit for turning collected security evidence into clear, prioritized reports.

Alice Community is built around a simple idea:

> Evidence in → prioritized security report out.

It does **not** run live scans, exploit systems, access credentials, delete logs, or attack infrastructure. It helps analysts, students, small teams, and security-minded builders review evidence they already collected and turn it into safer, more useful security reports.

---

## What Alice Community Does

Alice Community helps with:

* Parsing common security evidence files
* Reviewing scanner outputs
* Prioritizing findings
* Creating Markdown, JSON, and HTML reports
* Building evidence-review workspaces
* Keeping defensive safety boundaries clear
* Helping small teams understand what needs to be fixed first

Supported evidence types include:

* Nmap text/XML output
* Nessus/OpenVAS-style CSV exports
* Nuclei JSONL output
* Basic security evidence files
* Manually collected findings and notes

---

## What Alice Community Does Not Do

Alice Community is intentionally defensive and evidence-based.

It does **not**:

* Run autonomous commands
* Launch live scans
* Exploit systems
* Access passwords, tokens, cookies, browser data, keychains, or `.ssh`
* Delete logs or hide activity
* Move laterally across systems
* Hack back or attack scammers
* Perform unauthorized testing
* Replace a professional security assessment

Alice is designed to support lawful, authorized, human-reviewed cybersecurity work.

---

## Why This Exists

Small teams, students, solo developers, and local businesses often do not have access to expensive security platforms or dedicated security staff.

Alice Community gives them a safer starting point:

1. Collect evidence using tools they are already allowed to use.
2. Give that evidence to Alice.
3. Get a structured report with risks, explanations, and remediation steps.

This project is also the open-source community edition of a broader Alice Cyber product direction focused on defensive security, evidence review, and responsible AI-assisted analysis.

---

## Installation

### Option 1: Install From Source

```bash
git clone https://github.com/YOUR-USERNAME/alice-cyber-community.git
cd alice-cyber-community
python -m venv .venv
source .venv/bin/activate
pip install -e .
```

For Windows PowerShell:

```powershell
git clone https://github.com/YOUR-USERNAME/alice-cyber-community.git
cd alice-cyber-community
python -m venv .venv
.\\.venv\\Scripts\\Activate.ps1
pip install -e .
```

### Option 2: Install the Wheel

```bash
pip install alice_cyber_community-0.1.0-py3-none-any.whl
```

---

## Quick Start

Check the installed version:

```bash
alice-community --version
```

Create a sample evidence workspace:

```bash
alice-community workspace --output ./demo_workspace
```

Generate a report from evidence:

```bash
alice-community report --input ./demo_workspace/evidence --output ./demo_report
```

---

## Example Workflow

```text
1. You collect evidence from systems you are authorized to review.
2. You place the evidence inside an Alice workspace.
3. Alice parses the evidence.
4. Alice ranks and explains the findings.
5. A human reviews the output.
6. The final report is shared with the system owner.
```

---

## Safety Philosophy

Alice Community is built around defensive security principles:

* Evidence-based analysis
* Human review
* No autonomous exploitation
* No credential access
* No stealth behavior
* No destructive actions
* No hack-back behavior
* No unauthorized testing

Security tooling should reduce risk, not create new risk.

---

## Commercial Boundary

This repository is the community edition.

The following enterprise/commercial features are intentionally not included:

* Tenant isolation
* Enterprise authentication
* Customer trust portal
* Local API server
* Case database
* License manager
* Signed updates
* Secrets vault
* Deployment readiness checks
* Commercial service packaging

This keeps the open-source project useful while protecting the broader product direction.

---

## Contributing

Contributions are welcome if they support defensive, authorized, evidence-based security work.

Good contribution ideas:

* Add a safe parser
* Improve report formatting
* Add tests
* Improve documentation
* Add safe sample data
* Improve remediation wording

Not accepted:

* Exploit code
* Credential theft logic
* Stealth/evasion features
* Log deletion
* Hack-back tooling
* Autonomous scanning/execution
* Anything designed for unauthorized activity

Read `CONTRIBUTING.md` before submitting a pull request.

---

## License

This project is released under the MIT License.

See `LICENSE` for details.

---

## Author

Created by **Homar Gonzalez Vargas**.

Alice Cyber Community Edition is part of a larger effort to build safer, more transparent, defensive AI-assisted cybersecurity tools.

---

## Disclaimer

Alice Community is provided for educational and defensive security purposes only.

It does not guarantee that a system is secure. Reports generated by Alice should be reviewed by a qualified human before being used for business, legal, or security decisions.
::: 
