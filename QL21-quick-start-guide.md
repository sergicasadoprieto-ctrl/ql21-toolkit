# QL21 · Quick Start Guide

> QL21 is a lightweight framework for documenting research projects in a reproducible and transparent way. It uses Git and open text-based formats so that project records remain accessible over time. No programming experience is required.

---

## 1. Install the tools

**Layer 1 — Required formats & version control**

| Format / Tool | Purpose |
|------|---------|
| Markdown | Plain text format for logs, notes & reports |
| YAML | Metadata & frontmatter for all documents |
| BibTeX | Reference format for bibliography |
| LaTeX | Format for academic writing & final reports |
| [Git](https://git-scm.com/downloads) | Local version control & history |

> The tools listed below are suggestions rather than requirements. If your institution already provides equivalent solutions, you can continue using them. The main goal is to work with open formats and maintain a clear project history.

**Layer 2 — Recommended**

| Tool | Purpose |
|------|---------|
| [Obsidian](https://obsidian.md) | Write & organise Markdown docs |
| [VS Code](https://code.visualstudio.com) | Editor for YAML, Markdown & scripts |
| [Zotero](https://www.zotero.org) | Reference manager |
| [Pandoc](https://pandoc.org) | Convert Markdown to PDF/Word |

**Layer 3 — Optional (AI)**

AI tools can be useful for drafting, summarising, reviewing, or organising research materials. However, responsibility for the accuracy and interpretation of the content always remains with the researcher. For confidential or sensitive work, consider running models locally using Ollama. For confidential research, use [Ollama](https://ollama.com) locally.

---

## 2. Start a new project (30 min)

The purpose of the initial setup is simply to establish a consistent structure for project documentation. Most files can be completed gradually as the project develops.

```bash
git clone https://github.com/username/my-project.git
cd my-project
mkdir 00-governance 01-literature 02-framework 03-pilot 04-outputs 05-journal
```

Copy the templates from `02-framework/templates/`. Fill in the governance manifests in `00-governance/`. First commit:

```bash
git add .
git commit -m "feat: initialise project structure v0.1.0"
git push -u origin main
```

---

## 3. Daily workflow

The workflow is designed to leave a lightweight record of each working session. This makes it easier to resume work after a break, review decisions, and share progress with collaborators.

| When | What | Where |
|------|------|-------|
| Project start | Copy `TPL-PROJ.md`, rename, fill in | `03-pilot/` |
| Start of session | Copy `TPL-LOG.md`, rename, fill in | `03-pilot/logs/` |
| New insight | Copy `TPL-ZN.md`, rename, fill in | `05-journal/` |
| End of week | Copy `TPL-RPT.md`, rename, fill in | `03-pilot/` |
| End of session | Commit & push | — |

**Naming convention:** `{PREFIX}-{YYYYMMDD}T{HHmmss}-{AUTHOR}-1.00.md`

**End every session with:**
```bash
git add .
git commit -m "docs: add LOG session YYYY-MM-DD"
git push
```

---

## 4. Commit prefixes

| Prefix | Use for |
|--------|---------|
| `feat` | New template or artefact |
| `docs` | Log, note, report |
| `fix` | Correction |
| `chore` | Maintenance |
| `refactor` | Renaming or restructuring |

---

## 5. AI assistance (optional)

Attach these files at the start of every AI session:
- `user-manifest.yaml`
- `project-manifest.yaml`
- `governance-manifest.yaml`
- Last RPT from `05-journal/`

Use local Ollama for confidential research.

---

## 6. Project closure

When a project reaches a stable final state, create a version tag to identify the release that supports reports, publications, or archived outputs.

```bash
git tag -a v1.0.0 -m "Project closure: final version"
git push origin v1.0.0
```

→ Full guide: [D4 Best Practices Guide](./D4-best-practices-guide.md)

---
*QL21 · IMB-CNM-CSIC / UAB · 2026 · CC-BY 4.0*
