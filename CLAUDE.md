# Project Guidance for Claude Code

## About this repository

`HydrogenFinancials` collects financial profiles of public companies
exposed to the hydrogen economy. One Markdown file per company lives in
`companies/`. `README.md` is the index and methodology. `TEMPLATE.md`
defines the standard file layout. There is no application code.

## Editing rules

- **Individual research per company.** Every figure must come from a
  primary source (company IR, annual report, stock exchange filing) or
  a clearly-labelled secondary source with URL. **No batch scripts. No
  synthetic or estimated data.** If a figure is unknown, write
  "not disclosed".
- **Cite on every number.** Every material financial figure is followed
  by `[source](URL)` inline.
- **Currency.** Keep reporting currency; do not silently convert.
- **Latest available.** Each profile must state the latest full fiscal
  year reported and the latest reported quarter, with dates.
- **Wrap prose at ~78 characters.** Tables may exceed this.
- **British English** spelling; no emojis; no marketing language.
- **One file per company.** Do not split a company across multiple
  files or merge multiple companies into one file.

## Git workflow

- **Always commit and push directly to `main`.** No feature branches,
  no pull requests, no review waits. This applies to local, Web, and
  scheduled remote sessions.
- Commit messages: short imperative subject (≤72 chars), body if the
  change is non-obvious.
- One logical change per commit where practical.

## Things not to do

- Don't create `scripts/`, `tools/`, or any automation that produces
  company files in bulk.
- Don't fabricate or extrapolate numbers to fill gaps.
- Don't mix hydrogen pure-plays with unrelated industrial names unless
  the README explicitly broadens scope.
