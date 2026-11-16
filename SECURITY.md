# Security policy

This policy covers every repository in the Sohedra organization.

## Reporting a vulnerability

Please don't report a vulnerability in a public issue, pull request or discussion.

Report it privately in one of two ways:

- **GitHub (preferred):** open the affected repository's **Security** tab and choose **Report a
  vulnerability**. For Sohedra, that's
  [github.com/sohedra/sohedra/security/advisories/new](https://github.com/sohedra/sohedra/security/advisories/new).
- **Email:** [security@sohedra.com](mailto:security@sohedra.com), if you can't use GitHub.

Include what you found, how to reproduce it, the versions affected and the impact you expect.
Please write your report in English.

### If you use AI tools

- Say whether AI helped you find the issue or write the report.
- Confirm the issue yourself before you report it: reproduce it against our code.
- Don't paste an AI-generated explanation you haven't checked.

Reports that don't meet these rules may be closed without a reply.

## What happens next

- We acknowledge your report within 7 days. If you don't hear back by then, email
  [security@sohedra.com](mailto:security@sohedra.com).
- We confirm whether it's a vulnerability and keep you updated at least every 14 days while we
  work on a fix.
- We publish a GitHub security advisory when the fix is released, and credit you unless you'd
  rather stay anonymous.
- We aim to disclose within 90 days of your report. If a fix takes longer, we'll agree on a date
  with you.

Please give us that time before you disclose the issue publicly.

## What Sohedra trusts

Sohedra trusts the developer who uses it: their code, their configuration, and the packages they
install. A problem that needs control over any of those is not a vulnerability in Sohedra.

Sohedra does not trust data from outside the app's code: data from the network, and input from the
app's users. A way for that data to run code, reach data it shouldn't, or break a strict Content
Security Policy through our code is a vulnerability.

## Scope

In scope: vulnerabilities in code we publish, for example a component that renders unescaped
content, breaks a strict Content Security Policy or exposes data it shouldn't.

Out of scope:

- vulnerabilities in third-party dependencies that are already reported upstream
- problems that need an already compromised device or browser
- issues in your own application code that uses our packages
- features under `experimental` options: we fix their security bugs, but publish no CVE or advisory
  for them

## Supported versions

The latest minor version of each published package gets security fixes. After a new major version
ships, the previous major's last minor gets security and critical fixes for 6 months. A
repository's README says whether it has published anything yet.
