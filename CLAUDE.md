# CLAUDE.md - macrocue-embeds

Context for Claude sessions that open this repo on their own (phone and cloud sessions) with no access to Joe's Obsidian vault.

## Read this first

- This repo holds the served HTML embeds for macrocue.com. Public files only: everything committed here is publicly readable once served.
- `Code Drop\` on Joe's machines is the authoritative source for the embeds. Files here can lag it. Never state which version is live from this repo - the vault's Deployment Manifest is the only record.
- Changes land by pull request. Do not push to `main`.
- Transfer whole files, never retype or truncate them. After any change, check line count and byte size, then read the version marker back.
- Never put credentials, keys or tokens in any file, commit, PR text or chat.
- If a task needs the vault or the live-version record, stop and say so rather than guessing.

## Rules for served files

- Served files carry NO comments beyond a one-line identity marker on line 2: `<!-- MacroCue <Name> Embed vNN - YYYY-MM-DD - see MacroCue_Deployment_Manifest for history -->`. No internal commentary, caveats or reasoning in anything that gets served.
- Never change the nav embed id `#html15`.
- Use `' - '` (spaced hyphen), never em-dashes or unicode dashes - they break the embed JavaScript.
- en-US spelling in every user-visible string (realized, favor, color, analyzed). Code comments are exempt.
- Display rounding: use `Math.round(v * 10**n) / 10**n`, not `toFixed()`.
- When verifying, measure bytes with `new Blob([text]).size`, never `String.length`.

## Session naming

Name sessions `<Area> - <Topic> [Cloud]`, for example `MacroCue - Embed fix [Cloud]`. Areas: MacroCue, Career, Personal.
