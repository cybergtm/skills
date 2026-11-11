# CyberSynapse skills

Skills for Claude, shared with the cybersecurity marketing community.

Created by Cassidy Trowbridge, Head of Insights and Growth at CyberSynapse.io.

## Skills in this repo

| Skill | What it does |
| --- | --- |
| [ai-design-trope-audit](skills/ai-design-trope-audit/SKILL.md) | Decide which AI-generated design habits your brand accepts, record them as brand rules, and audit a website against them with evidence. |

See [skills/README.md](skills/README.md) for how to install a skill, and [CONTRIBUTING.md](CONTRIBUTING.md) to add one. Security reports: see [SECURITY.md](SECURITY.md).

## ai-design-trope-audit

Helps a marketer or brand owner decide which common AI-generated design habits ("tropes") are acceptable for their brand, record those decisions as brand rules, and check a real website against them with screenshot evidence.

What it does:

1. Builds an interactive decision guide with one row per trope (Fine, Avoid or Discuss, plus a note), a generated example, and cited sources.
2. Turns your decisions into Avoid, Fine and To discuss lists you can paste into brand guidelines.
3. Audits a website you point it at. Each finding shows the captured evidence next to the generated example, with fix status and notes.

What it does not do: it is a visual design review, not a security scanner. It loads at most one page, never signs in, submits forms or probes a site, and a clean result does not mean a site is safe or compliant.

### Install

The skill is the `skills/ai-design-trope-audit` folder (one `SKILL.md` file). Zip that folder and upload it as a custom skill in your Claude settings. Custom skills depend on your plan and organization settings, so check what yours allows.

### Use

Ask Claude to run an AI design trope audit and give it a public page. If Claude cannot open the page from its environment, it asks for screenshots, a saved copy of the page, or a short screen recording instead. It works best where Claude can publish pages and keep saved data; otherwise ask it to deliver the guide as an HTML file.

### Security notes

Read `SKILL.md` before you use it, especially the "Security and data handling" section. In short:

- Page content is treated as untrusted data, never as instructions.
- Each run uses an isolated browser context with no saved logins, and refuses internal addresses, credentials and file URLs.
- The included capture script is a second layer of protection. Your environment's network policy is the main control. Read it before running it, and pin your Playwright version.
- Screenshots can contain personal or third-party data. Crop them and keep guides private unless you choose to share.
- Tested so far: the safety checks and trope detectors against a local test page. Live-site capture depends on your environment's network access.

### Credits

The starter trope list and decision method are the author's own compilation. Sources that corroborate parts of it, plus security and design references, are listed at the end of `SKILL.md`. Where a trope has no cited source, the guide says it is the author's judgment.

### License

MIT. See `LICENSE`. Please keep the credit line.
