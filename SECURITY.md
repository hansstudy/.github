# Security Policy

## Supported versions

Only the latest published release of each project under `github.com/hansstudy` receives
security fixes. There is no long-term-support branch; upgrade to the latest release to pick up a
fix.

| Version | Supported |
|---|---|
| Latest release | yes |
| Anything older | no - upgrade first |

## Reporting a vulnerability

Please report suspected vulnerabilities privately, not in a public issue.

1. Preferred: use **GitHub private vulnerability reporting** on the affected repo
   (Security tab -> "Report a vulnerability"). It is enabled on every tool repo published here.
2. Alternative: email **bugs@hans.study**.

Please include: the affected repo and version/tag, a description of the issue, reproduction
steps or a proof of concept, and the potential impact. Do not include live credentials or
customer data in a report.

## Response window

Acknowledgement within **5 business days**. A fix or a mitigation plan within **30 days** for a
confirmed high/critical issue, longer for lower-severity findings, communicated back to the
reporter. This is a best-effort window from a solo maintainer, not a contractual SLA - see the
repo's own support statement.

## Scope

In scope: the code in this repository, its release workflow, and the artifacts it publishes
(GitHub Releases, PowerShell Gallery packages, scoop/winget manifests, Stream Deck plugin
packages, Claude Code plugin packages).

Out of scope: vulnerabilities in a vendor SDK, product, or platform this project integrates with
but does not vendor (report those to the vendor); social engineering; denial of service against
GitHub's own infrastructure; issues that require an already-compromised host to exploit.

## Disclosure

Coordinated disclosure preferred. Please allow the response window above to elapse (or a fix to
ship) before public disclosure. Credit is given in the release notes unless the reporter asks to
stay anonymous.
