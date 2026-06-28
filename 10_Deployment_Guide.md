# 10 — Deployment & Maintenance Guide

## Project

Personal Portfolio Website

Version 1.0

---

# Purpose

This document explains how to maintain, update and extend the portfolio without redesigning or restructuring it.

The project should grow over time while preserving its identity and architecture.

---

# Deployment

Platform

GitHub Pages

Branch

main

Root

/

No build process required.

After pushing changes to the main branch, GitHub Pages publishes the website automatically.

---

# Repository Workflow

Recommended workflow

Create feature branch

↓

Develop

↓

Test locally

↓

Commit

↓

Merge into main

↓

GitHub Pages deploys automatically

Avoid committing unfinished experiments directly to main.

---

# Folder Structure

Never change the main structure.

New content should be added inside existing folders whenever possible.

Example

projects/

new-project/

cover.webp

gallery/

project.json

README.md

Do not create new organizational patterns unless the current one becomes insufficient.

---

# Adding a New Project

1.

Duplicate an existing project folder.

2.

Rename the folder.

3.

Replace assets.

4.

Update project.json.

5.

Translate project content.

6.

Update project index.

Nothing else should require modification.

---

# Adding Images

Place images inside the corresponding project folder.

Recommended format

WebP

Maximum width

1920 px

Optimize before uploading.

Every image should replace an existing placeholder.

Never change layout dimensions.

---

# Updating Hero Portrait

Replace

assets/images/hero/alejandro-hero.webp

Use the same filename whenever possible.

This avoids unnecessary code changes.

Recommended checklist

✓ Transparent background

✓ Similar framing

✓ Similar composition

✓ Similar lighting

✓ Optimized WebP

---

# Updating the Resume

Replace

cv/resume-en.pdf

cv/resume-es.pdf

Never change filenames.

The portfolio always references these files.

---

# Updating Profile Information

Personal information should come from a central configuration file.

Example

config/profile.json

Contains

Name

Headline

Location

Email

LinkedIn

GitHub

Itch.io

Resume paths

Never duplicate this information.

---

# Updating Skills

Skills belong inside

data/skills.json

Never hardcode skills inside HTML.

Every section should consume the same source.

---

# Updating Experience

Modify

data/experience.json

Experience cards update automatically.

---

# Updating Education

Modify

data/education.json

Never edit HTML directly.

---

# Updating Timeline

Modify

data/timeline.json

Timeline should rebuild automatically.

---

# Updating Languages

Modify

locales/

en.json

es.json

Never edit translated HTML.

---

# Adding a New Language

Duplicate

en.json

Translate values.

Register language inside

config.js

Everything else should continue working.

---

# Theme Customization

Primary color

Defined once.

Example

--color-primary

Changing this variable should update the entire interface.

Avoid changing colors component by component.

---

# Typography

Change fonts only inside

tokens.css

Never redefine fonts locally.

---

# Icons

Store SVG files inside

assets/icons/

Do not mix icon libraries.

Keep a single visual style.

---

# Adding a New Section

Create

HTML component

↓

CSS

↓

JavaScript

↓

Translation

↓

Navigation entry

↓

Configuration flag

Sections should be removable without affecting the rest of the portfolio.

---

# Feature Flags

All optional content is controlled through

config.js

Example

ENABLE_BOOK

ENABLE_BLOG

ENABLE_EXPERIMENTS

ENABLE_WRITING

ENABLE_TIMELINE

ENABLE_TECHNOLOGIES

Changing one value enables or disables the entire feature.

---

# Future Book

Already planned.

Folder

content/book/

Contains

README.md

drafts/

images/

resources/

Leave disabled until ready.

---

# Future Blog

Folder

content/blog/

Markdown supported.

Each article contains

metadata

cover

content

translations

Disabled by default.

---

# Certificates

Store inside

assets/certificates/

Never embed full-size certificate images.

Use thumbnails.

Open full version only when requested.

---

# GitHub Integration

Repositories should be loaded from configuration whenever possible.

Avoid editing HTML to add repositories.

---

# Screenshots

Replace placeholders gradually.

The website should never break because an image is missing.

---

# Versioning

Use Semantic Versioning.

v1.0.0

Initial release

v1.1.0

New features

v1.1.1

Bug fixes

Maintain

CHANGELOG.md

---

# Performance Checklist

Before every release

✓ Compress images

✓ Check Lighthouse

✓ Test dark mode

✓ Test light mode

✓ Test translations

✓ Test mobile

✓ Validate links

✓ Validate downloads

✓ Validate accessibility

---

# Browser Checklist

Chrome

Edge

Firefox

Safari

Mobile Chrome

Mobile Safari

---

# Accessibility Checklist

Keyboard navigation

Visible focus

Alt text

ARIA labels

Reduced motion

Contrast

Screen readers

---

# SEO Checklist

Unique page titles

Unique descriptions

Open Graph

Twitter Cards

Structured Data

Canonical URLs

robots.txt

sitemap.xml

---

# Backup Strategy

Keep

Repository

↓

GitHub

↓

Local clone

↓

ZIP backup before major releases

Never depend on a single copy.

---

# Future Improvements

Possible future additions

CMS

Blog

Interactive demos

Project filters

Animations

Writing

Book

Talks

Courses

These additions should extend the portfolio.

Never replace its original philosophy.

---

# Maintenance Philosophy

Improve the portfolio the same way projects improve.

Small iterations.

Frequent refinements.

Thoughtful changes.

Never redesign everything because trends changed.

---

# Final Principle

This portfolio is a long-term product.

Treat it like software.

Keep improving it, but never lose the original idea:

Understand the problem before building the solution.
