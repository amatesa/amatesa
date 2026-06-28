# 00 — Document Index

## Purpose

This document is the master index for the entire project documentation.

It provides a complete overview of every document, its purpose, dependencies and implementation status.

Before reading any other document, review this index to understand how the documentation is organized.

This file is the primary navigation entry point for both human contributors and AI coding assistants.

---

# Documentation Structure

The documentation is organized into the following sections.

```text
docs/

00_READ_FIRST.md

vision/
experience/
content/
screens/
architecture/
planning/
assets/
```

Each section represents one layer of the project.

The documentation should be read from high-level vision toward technical implementation.

---

# Vision

These documents define why the portfolio exists.

They should be considered stable and rarely modified.

| Document                  | Purpose                                   | Depends On | Status |
| ------------------------- | ----------------------------------------- | ---------- | ------ |
| 00_Alejandro_DNA.md       | Personal values, motivations and identity | None       | Stable |
| 01_Vision.md              | Product vision                            | DNA        | Stable |
| 01_Portfolio_Narrative.md | Narrative structure                       | Vision     | Stable |
| 02_Brand.md               | Brand identity                            | Vision     | Stable |
| 13_Design_Principles.md   | Design philosophy                         | Brand      | Stable |

---

# Experience

These documents define how visitors experience the product.

| Document              | Purpose              | Depends On    | Status |
| --------------------- | -------------------- | ------------- | ------ |
| 14_UX_Blueprint.md    | UX principles        | Vision        | Stable |
| 15_Art_Direction.md   | Visual direction     | UX Blueprint  | Stable |
| 16_Motion_System.md   | Motion principles    | Art Direction | Stable |
| 17_UI_System.md       | Interface system     | Motion System | Stable |
| 18_Visual_Language.md | Visual communication | UI System     | Stable |
| 19_User_Journey.md    | Visitor progression  | UX Blueprint  | Stable |

---

# Content

These documents define what is communicated.

| Document                    | Purpose                        | Depends On       | Status |
| --------------------------- | ------------------------------ | ---------------- | ------ |
| 07_Content_Strategy.md      | Content strategy               | Vision           | Stable |
| 07_Portfolio_Copy_Master.md | Master copy and editorial tone | Content Strategy | Living |

---

# Screens

These documents define each major interactive section.

Read them sequentially.

| Document                | Purpose                    | Depends On | Status |
| ----------------------- | -------------------------- | ---------- | ------ |
| 20_Home_Screen.md       | Hero experience            | UX + UI    | Stable |
| 21_Think_Screen.md      | Thinking Workspace         | Home       | Stable |
| 22_Build_Screen.md      | Builder Workspace          | Think      | Stable |
| 23_Project_Workspace.md | Universal project template | Build      | Stable |

Future documents:

* 24_Learn_Screen.md
* 25_Explore_Screen.md
* 26_Connect_Screen.md

---

# Architecture

These documents define implementation.

| Document                         | Purpose                           | Depends On             | Status |
| -------------------------------- | --------------------------------- | ---------------------- | ------ |
| 03_Information_Architecture.md   | Information organization          | Vision                 | Stable |
| 04_Design_System.md              | Design tokens                     | UX                     | Stable |
| 05_Component_Library.md          | Components                        | Design System          | Stable |
| 06_Interaction_System.md         | Interaction rules                 | Component Library      | Stable |
| 08_Technical_Architecture.md     | Overall architecture              | Vision                 | Stable |
| 09_Asset_Guide.md                | Asset production                  | Art Direction          | Living |
| 10_Deployment_Guide.md           | Deployment process                | Technical Architecture | Stable |
| 11_Codex_Implementation_Guide.md | Development workflow              | Technical Architecture | Stable |
| 12_Codex_Master_Prompt.md        | Original implementation prompt    | Historical Reference   |        |
| 24_Content_Architecture.md       | Content organization              | Technical Architecture | Stable |
| 25_Content_Model.md              | Content entities                  | Content Architecture   | Stable |
| 26_Production_Blueprint.md       | Repository architecture           | Content Model          | Stable |
| 27_Engineering_Standards.md      | Engineering conventions           | Production Blueprint   | Stable |
| 28_Codex_Master_Instructions.md  | Final implementation instructions | Entire documentation   | Stable |

---

# Planning

Planning documents coordinate implementation.

They are operational documents rather than design documents.

Current documents

* 00_READ_FIRST.md
* 29_Implementation_Roadmap.md

---

# Assets

This section contains production resources.

It is expected to evolve continuously.

Recommended structure

```text
assets/

moodboard/

wireframes/

photography/

icons/

references/
```

---

# Reading Order

Every new contributor should follow this order.

1. 00_READ_FIRST.md

2. Vision

3. Experience

4. Content

5. Screens

6. Architecture

7. Planning

8. Assets

---

# Document Status

Stable

The document defines approved decisions.

Changes should be exceptional.

Living

Expected to evolve during development.

Historical Reference

Preserved for context.

Not considered the current source of truth.

---

# Source of Truth

If two documents appear to contradict each other:

1. 28_Codex_Master_Instructions.md
2. 27_Engineering_Standards.md
3. Screen specifications
4. Experience documents
5. Vision documents

If uncertainty remains, clarification should be requested before implementation.

---

# Maintenance

Whenever a new document is created:

* Add it to this index.
* Define its dependencies.
* Assign a status.
* Update the reading order if necessary.

This file must always reflect the current state of the documentation.
