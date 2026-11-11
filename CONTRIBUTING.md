# Contributing

Thanks for adding to this collection. Skills here are used by cybersecurity marketers, so the bar for safety and honesty is high.

## Checklist for a new or changed skill

- [ ] The folder name is lowercase with hyphens and matches the `name` in `SKILL.md`.
- [ ] The skill has a "Security and data handling" section covering untrusted content, scripts, network access, data exposure, approvals and limits.
- [ ] Any embedded script is short enough to read in full, uses only well-known libraries, writes only to a scratch folder, and does not download or run other code.
- [ ] The skill never asks for or enters credentials, and never signs in, submits forms or probes systems it was not asked to review.
- [ ] Sources are real, dated and linked. Claims without a source are labelled as the author's judgment. Nothing is invented.
- [ ] Generated examples are labelled as generated and never presented as real screenshots, quotes or data.
- [ ] Language is inclusive. Prefer blocklist and allowlist, primary and secondary, main for default branches, quick check instead of sanity check, and test value instead of dummy value.
- [ ] No private names, customer details, internal URLs, keys or tokens appear anywhere in the files.
- [ ] The root `README.md` and `skills/README.md` list the skill.

## Review

Open a pull request. A maintainer reads every line of any script and the security section before merging.

## Credit and license

Keep the author credit line in each skill. By contributing you agree your work is released under the MIT license in `LICENSE`.
