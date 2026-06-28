# 11 — CODEX Implementation Guide

## Project

Personal Portfolio Website

Version 1.0

---

# Objective

Implement the portfolio exactly as described in the documentation.

Do not reinterpret the design.

Do not simplify the architecture.

Do not replace design decisions with personal preferences.

If documentation conflicts with assumptions, always follow the documentation.

---

# Development Philosophy

Write production-quality code.

Assume this repository will be publicly available.

Every file should be readable.

Every folder should have a clear purpose.

Every component should be reusable.

The final product should look and feel like a professional open-source project.

---

# General Rules

Never duplicate code.

Never duplicate styles.

Never duplicate HTML structures.

Never hardcode repeated values.

Prefer reusable modules.

Prefer composition over repetition.

---

# HTML

Use semantic HTML5.

Prefer

header

main

section

article

aside

footer

nav

button

figure

figcaption

Avoid unnecessary div nesting.

Every page must have a logical heading hierarchy.

Only one H1 per page.

---

# CSS

Use modern CSS.

Prefer

Grid

Flexbox

Custom Properties

Clamp()

Container Queries where supported

Logical Properties

Avoid

!important

Deep selector nesting

Magic numbers

Hardcoded colors

Repeated spacing values

Every value should come from design tokens whenever possible.

---

# JavaScript

Use ES Modules.

No global variables.

No inline JavaScript.

Each file should have one clear responsibility.

Prefer pure functions.

Prefer immutable patterns.

Avoid large classes unless clearly justified.

---

# Folder Discipline

Each folder contains

README.md

Purpose description

Expected contents

Future extensions

Folder names should explain themselves.

---

# Naming

Use descriptive names.

Avoid abbreviations.

Good

project-gallery.js

Bad

gallery2.js

Good

project-card.css

Bad

styles-new.css

---

# Comments

Explain intent.

Not syntax.

Good

Why the gallery behaves this way.

Bad

Increment variable.

---

# TODO Comments

Every unfinished area includes structured TODOs.

Example

TODO:

Expected asset

Expected filename

Recommended dimensions

Replacement instructions

Priority

Future improvements

---

# Asset Comments

Every placeholder includes documentation.

Example

Expected image

Resolution

Aspect ratio

Purpose

Compression

Style

Lighting

Composition

Folder

Filename

Never leave generic placeholders.

---

# Configuration

Anything likely to change belongs in configuration.

Colors

Theme

Feature flags

Languages

Contact information

Navigation

Resume paths

Project list

Do not hardcode configurable values.

---

# Feature Flags

All optional sections must support

true

false

No code deletion required.

---

# Accessibility

Keyboard first.

Visible focus.

ARIA only when needed.

Screen reader friendly.

Reduced motion support.

Proper labels.

Skip navigation link.

---

# Performance

Lazy loading

Intersection Observer

Passive listeners

Responsive images

Minimal JavaScript

Minimal CSS

No unnecessary repainting

Optimize animations

---

# Animation

Animations use CSS whenever practical.

JavaScript only when interaction requires it.

Never animate layout if transform can achieve the same result.

Respect reduced motion.

---

# Images

Every image has

alt

width

height

loading

decoding

Optimized format

---

# SVG

Inline preferred.

Optimized.

Meaningful IDs.

No unnecessary metadata.

---

# Responsive

Desktop

Tablet

Mobile

No layout simply shrinks.

Every breakpoint reviewed individually.

---

# Internationalization

No duplicated HTML.

Everything translated through locale files.

Language switching without reload.

---

# Theme

Light

Dark

System

Stored locally.

No flicker during initialization.

---

# Developer Mode

Optional configuration.

Shows

Grid

Breakpoints

Component names

Spacing

Hidden placeholders

Disabled by default.

---

# Error Handling

Broken images

Missing translations

Missing project data

Invalid configuration

Graceful fallback.

Never crash the interface.

---

# Documentation

Every reusable module begins with a documentation block.

Purpose

Dependencies

Inputs

Outputs

Configuration

Extension notes

---

# Git Commits

Recommended style

feat:

fix:

refactor:

docs:

style:

perf:

chore:

---

# Code Quality

Readable.

Predictable.

Modular.

Consistent.

Documented.

Scalable.

Maintainable.

---

# Testing Checklist

Navigation

Theme

Languages

Projects

Responsive

Accessibility

Performance

404

Downloads

Contact links

Feature flags

Reduced motion

Every release should pass the checklist.

---

# Deliverables

CODEX should generate

Complete project structure

All HTML pages

CSS architecture

JavaScript modules

Translation files

Configuration

Placeholder assets

README files

Developer comments

Documentation

Deployment ready repository

No placeholder code should be undocumented.

---

# Final Principle

Write code as if another developer will maintain it for the next five years.

The implementation should reflect the same philosophy as the portfolio itself:

Understand first.

Build second.

Improve continuously.
