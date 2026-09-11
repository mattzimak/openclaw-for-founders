# OpenClaw field guide

{{header_line}}

One founder's field guide to running a company with an OpenClaw agent: the setup choices I made and why, the security rules I keep, the skills I install, the memory patterns that stuck, and the people worth learning from. It is not a directory of everything that exists - if something is here, it earned its place in real work. The longer notes live in [FIELD-NOTES.md](FIELD-NOTES.md). Suggest a link by opening an issue (see [CONTRIBUTING.md](CONTRIBUTING.md)).

Descriptions are my own notes where I wrote one. Where I only saved a link, the description is the repository's or the post's own summary. Ratings like `(Matt: 8/10)` are my personal scores.

## Contents

{{toc}}

{{start_here}}

{{sections}}

## Other useful lists

This list is deliberately short and opinionated. When you want the exhaustive version, these are the ones I actually open:

- [alvinreal/awesome-openclaw](https://github.com/alvinreal/awesome-openclaw) - the reference directory for the OpenClaw ecosystem: official projects, dashboards, deployment tooling, memory systems, alternative clients, plugins and channel integrations. Several hundred entries against the seventy or so here, so start there when you are looking for a category rather than a recommendation.
- [alvinreal/awesome-openclaw-tips](https://github.com/alvinreal/awesome-openclaw-tips) - thirty numbered tips on messages, Telegram, memory, reliability, cost, operations, automation and architecture, each with the failure it prevents and a prompt you can paste. The closest thing to this repo's field notes written by someone else, and it covers ground mine does not.
- [VoltAgent/awesome-openclaw-skills](https://github.com/VoltAgent/awesome-openclaw-skills) - 5,400+ skills filtered and categorised from the official registry. Use it as the index when you know the job you want done and need to find out whether a skill already exists.

The difference is intent, not quality: those are directories of what exists, this is a record of what I kept after using it. If a link appears in both, theirs will be more complete and mine will tell you whether it survived contact with real work.

## How this list is built

The source is a private Notion page where I keep notes while I work. A sync script in my workspace (`awesome-sync.py`, not in this repo) reads that page through the Notion API and keeps only the sections that are explicitly mapped as public - everything else stays private by default. It canonicalizes every URL (https only, tracking parameters dropped, `youtu.be` and `twitter.com` rewritten), drops links to private places (Notion, Google Drive, course platforms, local addresses), scans every string for secrets and private names, and writes three files: `data/links.csv` (one row per link), `data/notes.json` (the field notes) and `data/_report.md` (what was excluded and why).

From there everything is automated and reproducible from this repo alone:

- `tools/enrich.py` checks every link and writes `data/enrichment.json`: stars, license, last push and archive state from the GitHub API (renamed repositories are followed), titles from YouTube and X oEmbed, and a plain HTTP check with a browser user agent for everything else.
- `tools/build.py` renders this README and `FIELD-NOTES.md` from `data/` + `config/sections.json` + `templates/`. Links stay here, every note goes to the notes file, grouped by the same sections. Entries are sorted by name inside each section; the build is deterministic, so running it twice produces the same files.
- `tools/lint.py` fails on dead links, descriptions under 30 characters, duplicate names or URLs, non-https links, tracking parameters, links to private hosts, long dashes, placeholders, thin sections and broken table-of-contents anchors - in both files. Whatever it cannot fix on its own is listed under "Open decisions" in `data/_report.md`.
- A weekly GitHub Action (`.github/workflows/links.yml`) re-runs the checks and opens a pull request when either file changes. `data/_dead.md` lists what needs a human look.

Nothing in this README or in `FIELD-NOTES.md` is edited by hand. Fixes go to `data/overrides.json` (keyed by the entry id in `data/links.csv`, or by block id under `_notes` for a note) and the next build picks them up.

{{stats}}

## License

The content of this list (README, FIELD-NOTES and the files in `data/`) is licensed under [CC BY 4.0](LICENSE) - share and adapt it with attribution. The scripts in `tools/` are MIT licensed ([LICENSE-CODE](LICENSE-CODE)).
