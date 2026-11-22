# Contributing

ManoLink Technologies Limited builds proprietary software. This file is the
organisation-wide default: it applies to any repository of ours that does not
ship its own `CONTRIBUTING.md`.

## Our repositories are proprietary

- All source code, designs and documents in our organisation are proprietary and
  all rights are reserved. See each repository's `LICENSE`.
- Nothing in this file grants a licence to use, copy, modify, redistribute or
  sublicense our code, and opening an issue places no obligation on us.
- We do not accept unsolicited code contributions. Please do not open a pull
  request unless a maintainer has asked you to.
- Contributions are made only by people with an employment, contractor or other
  written agreement with the Company; unless that agreement says otherwise, the
  Company owns the work contributed.

## Access

Our product repositories are private, and access is by invitation from
ManoLink Technologies Limited.

| Team | Access | For |
| --- | --- | --- |
| Maintainers | Maintain | Core engineers: merge, release, manage settings |
| Reviewers | Read | Invited code, IP and licensing reviewers |
| Security | Triage | Invited security reviewers |

## Reporting bugs and asking for features

Use the issue templates in this repository — they apply to our public
repositories. Include the repository, version or commit, and what you expected to
happen. Our roadmap is internal, so an accepted request is not a commitment to
build it.

Never put secrets, keys, tokens, customer data or personal data in a public
issue. For anything security-related, follow [SECURITY.md](SECURITY.md) instead of
opening an issue.

## Workflow for invited contributors

1. Branch from the default branch with a `feature/…`, `fix/…`, `docs/…` or
   `chore/…` prefix.
2. Keep each change focused and write commit messages in the imperative
   ("Add refund guard", not "added stuff").
3. Add or update tests with every behaviour change and run them locally before
   pushing. CI must pass.
4. Open a pull request against the default branch and fill in the template.
5. A member of **Maintainers** reviews and merges. Our repositories squash-merge,
   so the pull request title becomes the commit message.

## House rules

- Never commit `.env` files, keys, tokens, credentials or customer data. Copy
  `.env.example` where one exists and use sandbox or test credentials only.
- If you add configuration, update `.env.example` and the README in the same pull
  request.
- Third-party code or assets need a licence that permits our use, and an entry in
  `THIRD_PARTY_NOTICES.md` where the repository has one.
- Changes touching authentication, payments, money movement or personal data need
  a **Reviewers** or **Security** review before merge.
- Wakarail stays sandbox-only: do not enable live money movement and do not point
  tests at production.
- Be direct and civil in review. Critique the change, not the person.

## Security issues

Do not report vulnerabilities in public. See [SECURITY.md](SECURITY.md).
