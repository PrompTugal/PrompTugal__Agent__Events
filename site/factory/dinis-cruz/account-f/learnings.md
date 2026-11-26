# cl-6.events: learnings

From events.b's history (history/PrompTugal__News__Events/board/team/events/debriefs/2026-11-18-handover.md) and this setup.

- The gate fails on an em dash anywhere in the built site, source titles included: `clean()` prints a source's em dash as an en dash, and /how/ says so. Raise a hype word in a source title with Dinis; never weaken the check.
- `src/assets/render.mjs` is the one renderer for the build and the browser (live.js): change event cards there, not in the build.
- The Algarve page gathers its towns' claims itself (the API has no `algarve` claims file). London-ready: a place outside Portugal gets "Beyond Portugal: <name>".
- Write REALITY.md entries with a quoted heredoc; take times from `date -u` or `git log`, not from memory (earlier entries ran ahead of the clock).
- To test live.js with Playwright, give Chromium the proxy with `bypass: 'localhost'`, or the local server answers 405. Each browser test sends real test events to the observability lane: say so to the conductor.
- The key tooling that account B used (sgit pki keygen) was refused by that environment's classifier. Here a key is made with openssl, and ssh-keygen needs `apt-get install openssh-client` in a fresh container.
- This session's `add_repo` with push for the work repository was denied by the permission classifier on 26 Nov (01:42Z). A read-only clone of a public repository works with git. Not worked around.
- Open from events.b: branch protection on `dev` with a required check and CODEOWNERS for `.github/**` and `scripts/**`, a tag ruleset, and the github-pages environment limited to `dev` (Dinis's, via status.json asks).
