# 17 — UI System

## Purpose

This document defines the interface system used across the portfolio.

Its objective is consistency.

Every page should feel like it belongs to the same product.

Every component should behave predictably.

Every layout decision should reinforce readability.

---

# Design Philosophy

The interface should disappear.

Content remains.

Interaction remains.

Ideas remain.

If users consciously notice the UI, it is probably trying too hard.

---

# Layout

Desktop

12-column CSS Grid

Maximum width

1440px

Reading width

760–820px

Content should rarely exceed this width.

Large screens should increase whitespace.

Never line length.

---

# Breakpoints

Mobile

≤640px

Tablet

641–1024px

Laptop

1025–1440px

Large Desktop

1441px+

Layout should adapt progressively.

Never create independent mobile layouts.

---

# Spacing System

Base Unit

8px

Allowed spacing values

4

8

12

16

24

32

40

48

64

80

96

128

Spacing should never be arbitrary.

If a value is needed outside the system, reconsider the layout.

---

# Radius

Small

8px

Medium

12px

Large

20px

Never use different corner radii without semantic purpose.

---

# Borders

1px

Soft contrast

Never decorative

---

# Shadows

Elevation communicates interaction.

Not hierarchy.

Small

Hover

Medium

Floating Panels

Large

Modal Workspaces

Never stack multiple shadows.

---

# Typography

Three families only.

Primary

Reading

Secondary

Headlines

Monospace

Code

Never introduce additional fonts.

---

# Reading

Paragraph width

60–75 characters

Maximum

85 characters

Never justify text.

Always left align.

---

# Components

Only create reusable components when they appear three or more times.

Avoid premature abstraction.

---

# Primary Components

Navigation

Section

Hero

Project Card

Case Study

Button

Icon Button

Timeline Node

Information Panel

Gallery

Footer

Language Switch

Theme Switch

Workspace Window

Three.js Canvas

---

# Component Behaviour

Every component owns one responsibility.

Never combine unrelated behaviors.

---

# Buttons

Buttons initiate actions.

Links navigate.

Never confuse both.

---

# Cards

Cards represent ideas.

Not decoration.

Cards expand.

They never flip.

---

# Images

Images explain.

Not decorate.

Every image should support nearby text.

---

# Icons

Icons reinforce recognition.

Never replace labels.

---

# Three.js Integration

Three.js is a layer.

Not the application.

DOM remains primary.

Canvas enhances understanding.

If JavaScript fails,

the content still works.

---

# Progressive Enhancement

Level 1

HTML

Everything readable.

---

Level 2

CSS

Everything beautiful.

---

Level 3

JavaScript

Everything interactive.

---

Level 4

Three.js

Everything immersive.

Every level should remain functional independently.

---

# Theme System

Every component supports:

Light

Dark

System

No exceptions.

---

# Internationalization

English

Spanish

Every component must support translation.

Never hardcode text.

---

# Accessibility

Keyboard first.

Mouse second.

Touch third.

Screen readers always supported.

Visible focus indicators.

Semantic HTML.

Correct heading hierarchy.

ARIA only when necessary.

---

# Responsive Behaviour

Desktop gains space.

Mobile gains simplicity.

Never remove information.

Only reorganize it.

---

# Navigation

Sticky.

Minimal.

Transparent until necessary.

Never occupies excessive vertical space.

---

# Hero

One screen.

Never taller.

Never shorter.

Visitors immediately understand where they are.

---

# Projects

Open inside immersive workspaces.

Avoid unnecessary page reloads.

Navigation should feel continuous.

---

# Performance

Target

95+

Lighthouse

Desktop

95+

Mobile

90+

Largest Contentful Paint

<2s

Interaction

Immediate.

---

# CSS Architecture

Use CSS variables.

Use utility classes only when appropriate.

Prefer semantic class names.

Avoid deeply nested selectors.

Maximum selector depth

Three levels.

---

# JavaScript

Modules.

Small files.

Single responsibility.

No global state unless necessary.

---

# Three.js Architecture

Independent module.

Never tightly coupled to content.

Can be disabled without breaking navigation.

---

# Naming Convention

Readable.

Explicit.

Predictable.

Examples

hero-title

project-card

timeline-node

language-switch

workspace-panel

Avoid abbreviations.

---

# Comments

Every major section begins with documentation.

Every asset placeholder includes:

Expected dimensions.

Expected style.

Expected purpose.

Example

<!-- HERO PORTRAIT

Expected:

PNG/WebP

Transparent background

Approx. 1800px height

Soft side lighting

Neutral expression

Looking slightly toward content

-->

Future contributors should understand every placeholder without external documentation.

---

# Future Scalability

Adding a new project should require:

One markdown file.

One cover image.

Optional media.

No structural modifications.

The system should grow naturally.

---

# Final Principle

The interface should feel engineered rather than assembled.

Every element exists because it solves a problem.

Nothing exists because it fills space.
