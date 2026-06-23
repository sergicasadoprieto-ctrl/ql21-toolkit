# 📓 QL21 Toolkit — The 21st Century Lab Notebook

> QL21 was developed as part of a Bachelor's Thesis at IMB-CNM-CSIC and the Universitat Autònoma de Barcelona, motivated by the practical documentation challenges encountered in experimental research environments.

![License](https://img.shields.io/badge/license-CC--BY--4.0-F57C00?style=flat-square)
![Institution](https://img.shields.io/badge/IMB--CNM-CSIC-263238?style=flat-square)
![University](https://img.shields.io/badge/UAB-2026-263238?style=flat-square)

**Author:** Sergi Casado Prieto · IMB-CNM-CSIC / UAB · 2026

**Full project:** https://github.com/sergicasadoprieto-ctrl/tfg-quadern-laboratori-21c

---

## What is this?

During the survey and literature review carried out for this project, one issue appeared repeatedly: researchers often develop effective experimental workflows, but the documentation supporting those workflows is frequently incomplete or inconsistent.

QL21 addresses that gap with a practical, reusable documentation framework informed by a survey of 113 researchers at UAB Campus.

---

## Documentation site

The QL21 toolkit is also available as a web page at:  
https://sergicasadoprieto-ctrl.github.io/ql21-toolkit/

---

## What is included

```text
ql21-toolkit/
├── README.md
├── LICENSE.md
├── poster-ql21-documentation-stack.png
├── survey-insights.md
├── docs/
│   ├── D4-best-practices-guide.pdf
│   └── QL21-quick-start-guide.pdf
├── manifests/
│   ├── user-manifest-template.yaml
│   ├── project-manifest-template.yaml
│   ├── governance-manifest-template.yaml
│   └── branding-manifest-template.yaml
└── templates/
    ├── TPL-LOG.md
    ├── TPL-ZN.md
    ├── TPL-RPT.md
    └── TPL-PROJ.md
```

---

## Survey findings

- Mean reproducibility difficulty: **3.08 / 5**
- Would adopt structured templates: **68.4%**

Full results in [survey-insights.md](survey-insights.md)

---

## How to use

**New to QL21?**   
Start with the [Quick Start Guide](docs/QL21-quick-start-guide.pdf).  
For the full documentation framework, see the [Guide of Best Practices](docs/D4-best-practices-guide.pdf).

**Without Git:** Download ZIP above.  
**With Git:**
```bash
git clone https://github.com/sergicasadoprieto-ctrl/ql21-toolkit.git
```

---
## Using with institutional systems

This toolkit is designed for Git-based workflows. If your institution uses a self-hosted Git server (GitLab, Gitea, or similar), redirect the remote after cloning:

```bash
git remote set-url origin https://your-institution-server/your project.git
git push -u origin main
```

If your institution uses a document management system such as OpenText or SharePoint, these platforms serve a different purpose than Git and can coexist. Use Git for daily documentation and traceability, and export final deliverables to your institutional system when required for formal approval or archival.

---

*KM-TFG-QL21 · © 2026 Sergi Casado Prieto · IMB-CNM-CSIC & UAB*
