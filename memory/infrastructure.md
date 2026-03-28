# SitoPresepi2 — Infrastructure Facts
> Established: 2026-03-28
> Owner-approved via proposal `backoffice/proposals/proposal-storage-url-remote-repository-github.md`
>
> This file documents non-secret infrastructure facts for discoverability.
> **Canonical source for remote URLs is always `git remote get-url origin` inside each repo.**
> This file must not override the repo config — it is a reference, not an authority.

---

## GitHub Organisation

| Field | Value |
|---|---|
| Organisation | `Ame-no-Mahitotsu` |
| Visibility | All repos are **private** |
| SSH auth | Key registered under `Fex329` GitHub account — has owner/collaborator access to `Ame-no-Mahitotsu` |

---

## Repositories

| Repo | Purpose | SSH Remote | HTTPS Remote |
|---|---|---|---|
| Hephestus | Governance, AI config, agent files | `git@github.com:Ame-no-Mahitotsu/Hephestus.git` | `https://github.com/Ame-no-Mahitotsu/Hephestus.git` |
| Tools | PM tooling (ticket.py, message.py, dashboard) | `git@github.com:Ame-no-Mahitotsu/Tools.git` | `https://github.com/Ame-no-Mahitotsu/Tools.git` |
| SitoPresepe | Site source code (Django + Next.js) | `git@github.com:Ame-no-Mahitotsu/SitoPresepe.git` | `https://github.com/Ame-no-Mahitotsu/SitoPresepe.git` |
| Docs | Project documentation | `git@github.com:Ame-no-Mahitotsu/Docs.git` | `https://github.com/Ame-no-Mahitotsu/Docs.git` |
| Backoffice | Operational records, ceremonies, handoffs | `git@github.com:Ame-no-Mahitotsu/Backoffice.git` | `https://github.com/Ame-no-Mahitotsu/Backoffice.git` |

> **Note:** `SitoPresepe` root clone (`development/presepi-site`) currently uses the HTTPS remote.
> Dominick recommends switching to SSH for agent push workflows — pending Owner decision (ISS pending).

---

## Local Workspace Layout

| Path | Repo |
|---|---|
| `c:\temp\ClaudeProjects\hephestus\` | Hephestus (root, pull-only) |
| `c:\temp\ClaudeProjects\backoffice\` | Backoffice (root, pull-only) |
| `c:\temp\ClaudeProjects\docs\` | Docs (root, pull-only) |
| `c:\temp\ClaudeProjects\development\tools\` | Tools (root, pull-only) |
| `c:\temp\ClaudeProjects\development\presepi-site\` | SitoPresepe (root, pull-only) |
| `c:\temp\ClaudeProjects\Office\{Agent}-Desk\` | Agent desk clones — development work only |

---

## Hosting (planned)

| Field | Value |
|---|---|
| Provider | DigitalOcean Frankfurt |
| Rationale | EU jurisdiction, GDPR compliant, cloud firewall (constitution 2026-03-12) |
| Domain | TBD — not yet registered |
| Environment URLs | TBD — not yet provisioned |
