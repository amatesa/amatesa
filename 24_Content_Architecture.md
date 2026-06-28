# 24 — Content Architecture

## Purpose

This document defines how every piece of content is organized inside the portfolio.

Content must remain completely independent from presentation.

The interface renders content.

It never contains content.

This architecture allows the portfolio to evolve for years without structural redesign.

---

# Core Principle

Separate:

Content

↓

Presentation

↓

Interaction

↓

Rendering

No layer should depend directly on another.

Every layer should have a single responsibility.

---

# Architecture Overview

```
portfolio/

│

├── content/

├── assets/

├── components/

├── styles/

├── scripts/

├── three/

├── config/

├── locales/

└── public/

```

---

# Content

Everything that Alejandro writes lives here.

```
content/

about/

projects/

thinking/

learning/

explore/

pages/

```

Nothing inside this folder contains HTML.

Only Markdown.

---

# About

```
content/about/

about.en.md

about.es.md

mindset.en.md

mindset.es.md

working-with-me.en.md

working-with-me.es.md

```

---

# Projects

Every project has its own folder.

```
content/projects/

portfolio/

whispering-woods/

interactive-audio/

dashboards/

python/

future-project/

```

Each project contains:

```
project.md

metadata.json

```

Optional:

```
gallery.md

timeline.md

notes.md

```

---

# Markdown Philosophy

Markdown should contain ideas.

Never presentation.

Never styling.

Never layout.

Example

```
# Problem

The project began because...

## Investigation

...

## Lessons

...

```

Presentation belongs elsewhere.

---

# Metadata

Every project has metadata.

Example

```
title

slug

language

date

status

tags

category

readingTime

heroImage

thumbnail

github

demo

featured

technologies

```

No content duplicated.

Metadata exists only once.

---

# Assets

Every visual resource belongs here.

```
assets/

projects/

images/

icons/

illustrations/

textures/

video/

documents/

fonts/

```

---

# Project Assets

Example

```
assets/projects/

whispering-woods/

cover.webp

hero.webp

gallery/

architecture/

video/

documents/

```

Every project follows exactly the same structure.

---

# Languages

Every translatable text lives here.

```
locales/

en.json

es.json

```

Never hardcode interface text.

Examples

```
Explore

Download Resume

Next Project

Previous

Read More

```

Everything comes from localization.

---

# Configuration

```
config/

navigation.json

social.json

theme.json

site.json

projects.json

```

Changing navigation never requires touching HTML.

---

# Three.js

Three.js remains isolated.

```
three/

core/

scenes/

objects/

materials/

shaders/

animations/

utilities/

```

Three.js never contains business content.

It visualizes content.

---

# Components

Every reusable UI element lives here.

```
components/

Hero

Navigation

Workspace

ProjectCard

Gallery

Footer

LanguageSwitcher

ThemeSwitcher

Timeline

```

Components receive content.

They never own it.

---

# Data Flow

```
Markdown

↓

Parser

↓

JSON

↓

Components

↓

DOM

↓

Three.js Enhancement
```

Everything follows one direction.

Never circular dependencies.

---

# Project Rendering

Every project uses:

```
Project Workspace

↓

Markdown

↓

Assets

↓

Metadata

↓

Rendered Experience
```

Adding a project never changes the renderer.

---

# Images

Every image follows naming rules.

```
cover.webp

hero.webp

thumbnail.webp

gallery-01.webp

gallery-02.webp

architecture.webp

```

Never:

image-final-final-v3.png

---

# Documents

```
resume-en.pdf

resume-es.pdf

case-study.pdf

documentation.pdf

```

Consistent naming.

Always.

---

# Icons

```
icons/

outline/

solid/

social/

system/

```

Never mix icon styles.

---

# Videos

```
video/

preview.mp4

demo.mp4

walkthrough.mp4

```

Poster images required.

---

# Versioning

Content evolves.

URLs do not.

Never rename slugs unnecessarily.

Maintain stable links.

---

# Scalability

The portfolio should support:

50+

Projects

10+

Years

Unlimited articles

Unlimited experiments

Without changing architecture.

---

# Search

Future search functionality should index Markdown.

Never HTML.

---

# RSS

Future blog support should consume Markdown automatically.

No additional content layer.

---

# AI Compatibility

Every Markdown file should be understandable by humans and AI.

Clear headings.

Consistent structure.

Semantic sections.

Future AI assistants should be able to summarize any project automatically.

---

# Comments for CODEX

Treat the portfolio like a static content platform.

Not a collection of pages.

Content is permanent.

Presentation evolves.

Never duplicate information.

Never hardcode repeated text.

Every new project should require only content and assets.

Everything else should happen automatically.

---

# Final Principle

A future redesign should require changing components.

Not rewriting content.

If content must be edited because the interface changed,

the architecture has failed.
