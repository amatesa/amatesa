# 08 — Technical Architecture

## Project

Personal Portfolio Website

Version 1.0

---

# Objective

The project must be maintainable.

Readable.

Scalable.

Framework-independent.

GitHub Pages compatible.

Every decision prioritizes long-term maintenance over short-term convenience.

---

# Technology Stack

HTML5

CSS3

Modern JavaScript (ES Modules)

No frameworks.

No build tools required.

No Node.js dependency.

No React.

No Vue.

No Angular.

No Bootstrap.

No Tailwind.

The project must work directly from GitHub Pages.

---

# Browser Support

Latest Chrome

Latest Edge

Latest Firefox

Latest Safari

Graceful degradation for older browsers.

---

# Repository Structure

/

index.html

/projects/

about/

assets/

css/

js/

data/

components/

docs/

cv/

locales/

favicon/

robots.txt

sitemap.xml

404.html

README.md

LICENSE

---

# Assets Structure

assets/

images/

hero/

projects/

gallery/

icons/

logos/

backgrounds/

textures/

videos/

documents/

Every folder contains a README describing:

Purpose

Expected files

Recommended formats

Recommended dimensions

Optimization guidelines

---

# CSS Structure

css/

tokens.css

base.css

layout.css

components.css

sections.css

animations.css

themes.css

utilities.css

responsive.css

No file should exceed approximately 600 lines.

Split before becoming difficult to navigate.

---

# JavaScript Structure

js/

app.js

config.js

navigation.js

theme.js

language.js

animations.js

gallery.js

projects.js

timeline.js

cards.js

accessibility.js

utils.js

Each module has a single responsibility.

---

# Data Layer

All content separated from presentation.

Project data stored as JSON.

Education stored as JSON.

Experience stored as JSON.

Skills stored as JSON.

Timeline stored as JSON.

Translations stored independently.

Never hardcode repeated content inside HTML.

---

# Internationalization

locales/

en.json

es.json

Every visible string must exist in translation files.

Never duplicate translated HTML.

Switch language without page reload.

Language detection:

Browser

↓

Local Storage

↓

English fallback

---

# Configuration

config.js

Contains:

Theme

Language

Feature Flags

Enabled Sections

Experimental Features

Developer Mode

Portfolio Version

No values duplicated elsewhere.

---

# Feature Flags

Example

ENABLE_BLOG

ENABLE_BOOK

ENABLE_WRITING

ENABLE_TIMELINE

ENABLE_TECH_STACK

ENABLE_EXPERIMENTS

ENABLE_EASTER_EGGS

Every optional feature controlled here.

---

# Project Pages

Every project uses the same template.

Shared layout.

Shared CSS.

Shared JavaScript.

Only project data changes.

---

# Reusable Components

Header

Footer

Section

Project

Gallery

Timeline

CTA

Contact

Navigation

Loaded dynamically.

Avoid duplicated HTML.

---

# Images

Preferred

WebP

Fallback

PNG

SVG

JPEG only for photography if required.

Lazy loading.

Width and height attributes required.

---

# Image Comments

Every image placeholder includes developer comments specifying:

Expected filename

Folder

Resolution

Aspect ratio

Compression

Recommended export settings

Purpose

Replacement instructions

---

# Video

Preferred

MP4 (H264)

Poster image required.

Optional WebM.

Videos lazy loaded.

Never autoplay with sound.

---

# Icons

SVG only.

Inline whenever practical.

No external icon fonts.

---

# Fonts

Self-hosted.

WOFF2 preferred.

Fallback stack required.

Avoid Google Fonts requests.

---

# Accessibility

Semantic HTML.

ARIA only when necessary.

Keyboard navigation complete.

Reduced Motion supported.

Focus management.

Landmarks.

Proper heading hierarchy.

---

# SEO

Meta tags.

Open Graph.

Twitter Cards.

Structured Data (JSON-LD).

Canonical URLs.

robots.txt

sitemap.xml

Meaningful URLs.

Readable page titles.

Unique descriptions.

---

# Performance

Target Lighthouse:

Performance 95+

Accessibility 100

Best Practices 100

SEO 100

No unnecessary JavaScript.

Critical CSS.

Lazy loading.

Deferred scripts.

Compressed assets.

---

# Error Handling

404 page.

Broken image fallback.

Missing project fallback.

Translation fallback.

Graceful degradation.

---

# Logging

Production:

No console noise.

Development mode:

Helpful logging only.

No debugging leftovers.

---

# Code Style

Meaningful variable names.

Meaningful function names.

Small functions.

Pure functions whenever possible.

Early returns.

Minimal nesting.

Consistent formatting.

---

# Comments

Comments explain:

Why.

Never:

What.

Every placeholder must explain:

Expected asset.

Purpose.

Replacement instructions.

Future improvements.

TODO items.

---

# Developer Experience

A new developer should understand the project within 30 minutes.

Folder names should be self-explanatory.

Every major folder includes README.md.

Every reusable component documented.

---

# Documentation

Repository includes:

Architecture

Setup

Deployment

Customization

Adding Projects

Adding Languages

Replacing Assets

Performance Guide

Accessibility Guide

---

# Deployment

GitHub Pages.

No server required.

No backend.

Everything static.

Deploy directly from main branch.

---

# Versioning

Semantic Versioning.

v1.0.0

Every release documented.

Changelog maintained.

---

# Final Principle

The project should feel like a professional open-source product.

Not a personal website.

Someone discovering the repository should think:

"This project is exceptionally well organized."
