# Hermes skill tap: open-meteo-briefing

An original Hermes skill written for CSCI 599 Assignment 3 (the skill-publication option, A3 §7.2).
It produces a two-line weather briefing for any city from the free, keyless
Open-Meteo API, using only Hermes' built-in `web_extract` tool.

## Install

```bash
hermes skills install <github-user>/<this-repo>/skills/open-meteo-briefing

# optional: add the repo as a tap, to browse and update its skills with `hermes skills search`
hermes skills tap add <github-user>/<this-repo>
```

Requires the `web` toolset (`web_search`/`web_extract`) with a configured web
backend. Installs from a new tap get `community` trust, so Hermes runs its
security scan and shows a third-party warning on first install.

## Try it

> What's the weather in Pasadena today?

Expected: one or two lines, for example
`Today in Pasadena: partly cloudy, 24/14°, 10% rain. (Open-Meteo)`

## Publishing (for the student)

1. Create a public GitHub repo and copy this folder's contents into it (`skills/` at the root).
2. Set `author:` in `SKILL.md` to your name, and commit.
3. On a scratch Hermes install, run the install commands above and the test prompt;
   record the output for your evidence.
4. Submit the repo URL, the commit hash and the transcript. A public GitHub tap is an accepted
   destination for Hermes (so are ClawHub and skills.sh); a direct SKILL.md URL is not.
   From the reference repo, `bash local/verify-skill-publication.sh <user>/<repo>` records the
   fresh install and one run in `evidence/skill-publication-transcript.txt`.

License: MIT.
