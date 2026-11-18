# NEXUS Principal Engineer

Repo-architect demo by AntManThePro: a simulated principal-engineer agent
working a codebase — task runner with presets (bugfix / feature / refactor /
audit / training), a live agent log, a repo dependency graph on canvas, and
health metrics (correctness, reliability, security, maintainability).

- **Demo, honestly labeled:** the agent log, graph nodes/links, and metric
  values are simulated in-browser (Math.random drives the simulation).
  Nothing here measures a real repo; the demo labels say so on the page.
- **Saves:** none. No localStorage/sessionStorage, no backend, no fetch
  calls. The "download artifact" button exports the demo output as a file.
- **Dependencies:** Tailwind CDN, Font Awesome CDN, Google Fonts — the page
  needs internet for full styling, like the original.

## Which variant this is

Four Principal Engineer files exist across the batches. This build is the
cleaned copy `14-index.html` (69K, 1,482 lines, md5-identical to
`workspace/nexus-principal-engineer-clean/index.html`), cleaned Nov 6: zero
banned-branding hits, demo data labeled, working download button. The
others were rejected:

- `nexus-principal-engineer.html` (68K) — the pre-clean original, 1
  godmode2025.net hit.
- `NEXUS_Principal_Engineer_Artifact_v2.html` (89K) — NOT a newer build. It
  is a browser-saved copy of the same app: missing DOCTYPE, extension
  attributes, Tailwind compiled inline, pre-rendered runtime log lines,
  and inflated metric values (99/96/100/92 vs the cleaned copy's
  94/89/97/82). Same app, worse packaging.
- `nexus-principal-evolution-v2.html` (Drive, 69,872 bytes) — a different
  app ("PRINCIPAL EVOLUTION v2", 2,673 diff lines), not a Principal
  Engineer variant; left alone.

Only packaging changes were made here: the Nov 6 icon set was moved into
`icons/` with standard names, `<head>` icon links and `manifest.json`
updated to point at them. No code changes.

## Live

https://principal-engineer.netlify.app/

## How to use

1. Open the live site.
2. Pick a task preset — bugfix, feature, refactor, audit, or training — and run it.
3. Watch the agent log and the repo graph while the (simulated) agent works.
4. Check the health metrics, then download the artifact if you want the output.

Everything on the page is a demo: the log, graph, and metrics are simulated in the browser. Nothing here measures a real repo.

## Links

- Live site: https://principal-engineer.netlify.app/
- NEXUS World Hub: https://nexus-world-hub.netlify.app/
- Repo: https://github.com/AntManThePro/principal-engineer
