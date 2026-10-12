# Electron Publish Pro

> Find what blocks a signed release of your Electron app, then fix it.

Electron Publish Pro checks an Electron project the way a release would: code signing, macOS notarization, Windows signing, security settings, Mac App Store and Microsoft Store requirements, and auto-update. Every issue comes with a concrete fix. **Free during the beta.**

## Run a check

**On the web:** sign in at [electronpublish.com](https://electronpublish.com), connect a GitHub repo and run a Release Readiness Check.

**From your terminal, CI or an AI agent:**

```bash
npm install -g electron-publish-pro

epp login                                        # your electronpublish.com email and password
cd my-electron-app
epp init --goal direct --platforms macos,windows
epp check                                        # or: epp check --json --fail-on fail
```

The CLI reads files from the current folder, so it works with any git host and with uncommitted changes. Run `epp files` to see exactly what is sent.

## Repositories

| Repository | What it is |
|---|---|
| [`cli`](https://github.com/electron-publish-pro/cli) | The `epp` command-line tool · [npm: `electron-publish-pro`](https://www.npmjs.com/package/electron-publish-pro) |
| [`docs`](https://github.com/electron-publish-pro/docs) | Documentation |

## What's live and what's next

| | Status |
|---|---|
| Release Readiness Check (web) | ✅ Live |
| `epp` CLI with `--json` output for CI and AI agents | ✅ Live |
| Signed and notarized macOS builds | 🗳️ [On the roadmap](https://electronpublish.com/roadmap) |
| Windows code signing | 🗳️ [On the roadmap](https://electronpublish.com/roadmap) |
| Publishing to GitHub Releases, Mac App Store and Microsoft Store | 🗳️ [On the roadmap](https://electronpublish.com/roadmap) |

Vote on the roadmap for what you need; the most-wanted parts get built first.

## Links

- 🌐 [electronpublish.com](https://electronpublish.com)
- 📖 [Documentation](https://electronpublish.com/docs)
- 🔒 [Security](https://electronpublish.com/security)
- ✉️ hello@electronpublish.com
