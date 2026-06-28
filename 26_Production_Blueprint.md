# 26 — Production Blueprint

## Purpose

This document defines the implementation architecture of the portfolio.

Unlike previous documents, this file is written for developers.

Its purpose is to remove implementation ambiguity.

Every folder, module and responsibility should be clearly defined before development begins.

---

# Technology Stack

Build Tool

Vite

Language

HTML5

CSS3

Modern JavaScript (ES Modules)

3D

Three.js

Markdown Parser

Marked.js (or equivalent)

Animation

GSAP

Icons

Tabler Icons

Deployment

GitHub Pages

Analytics

Plausible (optional)

No framework should be introduced unless it solves a real problem.

---

# Architecture Philosophy

The project follows a modular architecture.

Each module owns one responsibility.

Business logic never mixes with presentation.

Three.js never owns content.

Markdown never owns layout.

Everything communicates through well-defined interfaces.

---

# Project Structure

src/

assets/

components/

content/

data/

layouts/

pages/

scripts/

styles/

three/

utils/

config/

public/

docs/

---

# assets/

Contains every static asset.

images/

icons/

illustrations/

fonts/

textures/

videos/

documents/

projects/

No generated assets belong outside this folder.

---

# components/

Reusable interface components.

Hero

Navigation

Footer

Workspace

ProjectCard

Timeline

ThemeSwitcher

LanguageSwitcher

Gallery

Modal

Button

Badge

Tag

Card

Section

Every component has:

HTML

CSS

JS

Optional documentation

---

# content/

Markdown only.

No HTML.

No CSS.

No JavaScript.

Content survives redesigns.

---

# data/

Configuration.

JSON.

Examples

navigation.json

social.json

projects.json

settings.json

---

# layouts/

Responsible for assembling pages.

Home

Project

Article

Resource

Layout never contains business logic.

---

# pages/

Entry points.

index.html

404.html

Nothing else.

Navigation is client-side.

---

# scripts/

Application logic.

app.js

navigation.js

theme.js

language.js

content-loader.js

workspace.js

animations.js

No file exceeds 400 lines whenever reasonably possible.

---

# styles/

CSS Architecture

tokens/

base/

layout/

components/

utilities/

themes/

animations/

No gigantic stylesheet.

Everything modular.

---

# three/

Completely isolated.

core/

camera/

scene/

renderer/

objects/

materials/

animations/

interactions/

loaders/

helpers/

Three.js should be removable without breaking content.

---

# utils/

Generic utilities.

Never business logic.

Examples

debounce

throttle

viewport

math

storage

fetch

---

# config/

Application configuration.

Site title

Social links

Default language

Theme

Animation settings

Performance settings

Everything configurable.

---

# Rendering Flow

Browser

↓

Load HTML

↓

Load CSS

↓

Load Core JS

↓

Load Markdown

↓

Render Components

↓

Initialize Three.js

↓

Enhance Experience

Content always appears before enhancements.

---

# Performance Strategy

Critical CSS inline.

Images lazy loaded.

Three.js deferred.

Videos on demand.

Markdown cached.

Fonts preloaded.

Never block first render.

---

# Three.js Loading

Home Scene

↓

Think Scene

↓

Build Scene

↓

Learn Scene

↓

Explore Scene

↓

Connect Scene

Scenes loaded only when necessary.

Destroy unused GPU resources.

---

# Responsive Strategy

Desktop

Full experience

Tablet

Simplified interaction

Mobile

Content-first

Three.js simplified

No duplicated layouts.

Only adaptive behavior.

---

# CSS Naming

Semantic.

Examples

hero-title

project-card

workspace-panel

navigation-item

Never

box1

container2

left-panel-final

---

# JavaScript Rules

ES Modules only.

No global variables.

No inline scripts.

No anonymous business functions.

Single responsibility.

---

# State Management

Keep it simple.

Current language

Current theme

Current workspace

Current project

Animation preferences

Reduced motion

Nothing more.

---

# Asset Naming

hero-portrait.webp

project-cover.webp

gallery-01.webp

timeline-node.svg

Never:

IMG_001.png

final-v3.png

---

# Accessibility

Semantic HTML

Keyboard navigation

ARIA when required

Visible focus

Reduced motion

Proper headings

Alt text mandatory

Accessibility is part of implementation.

Not a final task.

---

# Lighthouse Targets

Performance

95+

Accessibility

100

Best Practices

100

SEO

100

These are engineering requirements.

Not optional goals.

---

# Git Strategy

main

Production

develop

Integration

feature/*

Individual features

No direct commits to main.

---

# Comments

Every module begins with documentation.

Every exported function explains:

Purpose

Parameters

Returns

Side effects

Future contributors should understand the project without external documentation.

---

# Final Principle

The codebase should feel as organized as the interface.

Reading the repository should communicate the same values as using the portfolio.

Understanding first.

Structure second.

Implementation third.
