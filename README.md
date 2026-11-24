<div align="center">

# 🚀 TitanEd Orbit

### TitanEd's managed, AI-centric learning platform built on Open edX

**Product owner:** TitanEd &nbsp;·&nbsp; **My role:** Software Engineer at TitanEd (frontend) &nbsp;·&nbsp; **Aug 2025 – Present**

![React](https://img.shields.io/badge/React-20232A?style=flat&logo=react&logoColor=61DAFB)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)
![Redux](https://img.shields.io/badge/Redux-764ABC?style=flat&logo=redux&logoColor=white)
![Open edX](https://img.shields.io/badge/Open%20edX-02262B?style=flat)
![SCSS](https://img.shields.io/badge/SCSS-CC6699?style=flat&logo=sass&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)

</div>

> **Note:** TitanEd Orbit is a commercial product and its source code is private. This repository is a **project showcase**: what
> the product does, what I built and how. It contains no company code.

---

## 📌 About the product

TitanEd Orbit connects course creation (**Studio**), learning (**LMS**), AI assistance (**TitanAI**) and administration
(**Control-Hub**) in one platform, offered to institutions by subscription. Standard Open edX looks dated, is hard to brand for
each customer and gives teachers few planning tools. Orbit fixes that without forking Open edX.

## ✅ What I built

Frontend of **Studio and the LMS** across all **11 Open edX micro-frontend apps**:

| Area | What it does |
|---|---|
| 🎨 **Branding and theming system** | Each institution gets its own look across every app (see below) |
| 📅 **Instructor dashboard in Studio** | Calendar, assignments, widgets and graphs: a teacher's whole workload in one place |
| 🧭 **Templates, shared header and footer** | Ready-made platform templates; all 11 apps look and work like one product |
| 🌐 **Multilingual public site** | A landing site for each institution, connected to live course data |
| 📣 **Announcement banners and in-app feedback** | Platform-wide messages and direct user feedback, from a shared component library |
| 🔁 **Old/new interface switch** | Institutions move to the new interface at their own pace |
| ✉️ **Bulk email and ORA grading** | Redesigned to match the Orbit look and layout |
| ⬆️ **Upgrade to Open edX Verawood** | All 11 apps upgraded through plugins and plugin slots, never forks |
| 🛡️ **Quality** | Sentry error monitoring, plus ongoing fixes to navigation, layout, dark mode, translations and date/time inputs |

## 🎨 The branding and theming system

Every institution wants Orbit to look like its own. I built the system that makes this possible: its admins manage their brand
from Control-Hub, and the system carries it into every screen of Studio, the LMS, sign-in, dashboards and public pages.

**How it works**
- **Three levels:** brand settings (colours, fonts, text sizes, spacing, page width) → 40+ shared components with all their
  states (hover, active, disabled, focus) → small per-app layers for each of the 11 apps. One change reaches every app together.
- **Light and dark mode:** every brand setting has a dark-mode counterpart, created and checked automatically.
- **Theme creator:** templates, key colours and custom fonts (with upload), live preview across the apps before saving,
  change history with undo, and theme export and import.
- **Quality gate:** 22 automatic checks on every build and commit (colour contrast, button and focus states, fonts, screen sizes,
  right-to-left layout, dark mode, CSS size), so no brand can make the platform hard to read.

**Result:** a new institution's brand goes live in minutes instead of days of development, stays accessible and survives upgrades.

## 🏗️ How it's built

```
          ┌─────────────────────── TitanEd Orbit ───────────────────────┐
 Learner ─┤  LMS: Learning · Dashboard · Profile · Account · Discussions │
          │  Multilingual public site                                    │
 Teacher ─┤  Studio + TitanAI + Instructor dashboard                     │
          │  Gradebook · ORA Grading · Bulk email                        │
          ├──────────────────────────────────────────────────────────────┤
          │  Branding & theming system · Shared header/footer · Banners  │
          ├──────────────────────────────────────────────────────────────┤
          │  Open edX (Verawood) · Tutor · Docker                         │
          └──────────────────────────────────────────────────────────────┘
```

- **Frontend:** React, TypeScript, Redux, Paragon, SCSS
- **Extension approach:** Frontend Plugin Framework slots, Tutor plugins, a shared TypeScript component library
- **Theming:** Paragon design-token architecture, Style Dictionary, automated validation
- **Platform and quality:** Open edX (Verawood), Tutor, Docker on Ubuntu, Sentry, Jest, React Testing Library

## 👤 My role

Software Engineer, frontend: built the Studio and LMS features above and the branding and theming system end to end, took them
from design to production with the backend and product teams, and carried every app through the Verawood upgrade.
About 140 pull requests on this product.

[🤖 TitanAI, the AI inside TitanEd Orbit](https://github.com/sonukumarsingh01/titanai-learning-assistant)

---

<div align="center">

**Sonu Kumar** · Software Engineer · [LinkedIn](https://www.linkedin.com/in/dr-sonu-kumar/) · [GitHub](https://github.com/sonukumarsingh01)

</div>
