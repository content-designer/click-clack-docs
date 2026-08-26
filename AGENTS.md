# Documentation project instructions

## About this project

Customer-facing Click Clack documentation, hosted on Mintlify. The site exists so a writer can export a signed history and a publisher, editor, or platform can check that file without a Click Clack account.

- Pages are MDX with YAML frontmatter
- Configuration lives in `docs.json`
- The independent verifier is `@click-clack/provenance-verifier` on npm (Apache-2.0). Document `npm install --global @click-clack/provenance-verifier`, then `click-clack-verify`.

## Audience

Ideal customer: writers who need proof — people who will be asked by a publisher, an editor, or a platform what AI contributed. Secondary reader: that publisher/editor/platform, following [Check a receipt](/check-a-receipt) with no login.

## Terminology

- **Figment**, not agent, in customer-facing copy
- **Signed history** / **receipt** for the JSON export; **Markdown** for the manuscript download
- **Verified**, never “trusted”, for a passing cryptographic check
- **Click Clack**, never `ClickClack` or `Click Clack AI`

## Style preferences

- Active voice, second person
- Sentence case headings
- Bold for UI elements: **Download signed history**
- Code formatting for commands, files, and flags
- Do not overclaim: `operatorIndependentNonRepudiation` is always false; a paste proves paste only; a Bitcoin `confirmed` label is not authority

## Content boundaries

Do not publish internal operator material: `superpowers/`, production runbooks, privacy-for-pilots, evals, or design-system implementation notes. This site is receipts and how to check them.
