# Security policy

This is the organisation-wide security policy for **ManoLink Technologies
Limited**. It applies to every repository, website and published endpoint of ours
that does not ship a security policy of its own.

Our product source code is private and proprietary. Access is by invitation only.

## Reporting a vulnerability

Please report suspected vulnerabilities privately by email to
**hello@wakabots.com** with the subject line `SECURITY: <repository or site>`,
for example `SECURITY: wakarail-payment-engine`.

- Do not open a public issue, pull request or discussion about it, and do not
  publish it elsewhere.
- Do not include live credentials, API keys or customer data in your report.
  Redact them; if a secret is genuinely needed to reproduce, we will agree a
  private channel with you.
- Do not access, change, move or delete data that is not yours, and do not test
  against production systems without written permission from us.
- Test only accounts and data you created yourself.

### What to include

- A summary of the issue and the impact you expect.
- The affected repository, page or endpoint, and the commit, version or date.
- Reproduction steps or a proof of concept, and any relevant logs.
- How you would like to be credited, or tell us to keep you anonymous.

## Scope

In scope: source code in our public repositories, our public websites, and any
endpoint we publish as sandbox or demo.

Out of scope:

- Third-party services we use — please report those to the provider.
- Volumetric denial-of-service testing and automated load against our systems.
- Scanner output with no demonstrated, exploitable impact.
- Missing hardening that has no practical effect.
- Reports about the contents of private repositories: you should not have access
  to them in the first place.

Wakarail is **sandbox-only**: live money movement stays disabled until
regulatory authorisation, provider agreements and an independent security review
are complete. Testing that attempts to move real money or to reach real customer
accounts is never authorised.

## What you can expect

- We acknowledge reports within five business days.
- We keep you informed while we investigate, and tell you when a fix ships where
  we can.
- We credit you in the fix, release notes or a security acknowledgement if you
  would like that.
- We do not currently run a paid bounty programme.

Please give us reasonable time to fix the issue before you publish anything about
it. We will not pursue legal action over good-faith research that follows this
policy. That assurance does not cover extortion, data theft, privacy violations
or disruption of our services.

## Supported versions

Only the latest commit on the default branch of each active repository is
supported. Fixes are not back-ported to older commits or releases, and archived
repositories are unsupported.

## Repositories with their own policy

Where a repository ships its own `SECURITY.md`, that file takes precedence over
this one. Product repositories also describe how callbacks, keys and identifiers
are protected in their README.
