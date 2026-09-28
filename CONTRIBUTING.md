# Contributing

Thanks for the interest. This is published as working software, not as a supported product (see
the repo's own support statement) - contributions are welcome, reviewed when time allows, and
held to the bar below.

## Before you start

- For anything beyond a small fix, open an issue first describing the problem and your proposed
  approach, so you don't spend time on something that will not be accepted.
- Check `SECURITY.md` if what you found is a vulnerability rather than a bug - do not open a
  public issue for that.

## Build and test

Build and test instructions are runtime-specific and live in the repo's own `README.md` (a
`RequiredModules`/`RequiredVersion` PowerShell module, an `npm ci && npm test` Node project, and
a Stream Deck plugin's `streamdeck validate` step all differ). If this file is overridden with a
runtime-specific build section, that section replaces this paragraph and nothing else in this
file changes.

## Commit style

- One logical change per commit. Write the commit message in the imperative mood ("Fix X", not
  "Fixed X" or "Fixes X").
- Reference the issue number when one exists.
- Update `CHANGELOG.md` under `Unreleased` for any user-visible change.

## Developer Certificate of Origin

Every commit must be signed off:

```
git commit -s -m "..."
```

This adds a `Signed-off-by: Your Name <you@example.com>` trailer, certifying you wrote the
change or otherwise have the right to submit it under this project's licence
(<https://developercertificate.org/>). Pull requests with unsigned commits will be asked to
amend before merge.

## What will be accepted

- Bug fixes with a clear reproduction.
- Documentation fixes.
- Features that fit the project's stated scope in its README - open an issue first for anything
  larger.
- Tests.

## What will not be accepted

- Changes that add a runtime dependency without discussion first (dependency pinning and SBOM
  accuracy are release gates - see `docs/RELEASE-CHECKLIST.md` in the repo).
- Changes that add telemetry, phone-home behaviour, or a third-party analytics SDK (none by
  default is a hard rule, not a preference).
- Vendored copies of vendor SDKs, DLLs, headers, or sample code.
- Copied third-party standards/benchmark prose (see `docs/content-provenance.md` in the repo you
  are contributing to).
