# Screen 20 — Home

## Purpose

The Home screen is the first impression of the portfolio.

Its objective is not to explain who Alejandro is.

Its objective is to create curiosity.

Visitors should immediately feel they are entering a carefully designed interactive product rather than a conventional portfolio.

Everything should communicate confidence through simplicity.

---

# UX Goal

Visitors should think:

"This feels different."

Not because of visual effects.

Because every element appears intentional.

The Home screen should create enough curiosity that visitors naturally continue scrolling.

---

# Emotional Goals

Primary

Curiosity

Secondary

Trust

Precision

Calm

Never:

Urgency

Entertainment

Marketing

---

# Viewport

Desktop

100vh

Nothing important below the fold.

The first screen must feel complete.

Scrolling reveals a new chapter.

It never finishes the first one.

---

# Composition

The composition follows a two-column layout.

Left:

Human.

Right:

Ideas.

This balance represents Alejandro himself.

One side communicates personality.

The other communicates thinking.

Neither dominates.

---

# Navigation

Position

Top

Behavior

Sticky after first scroll.

Transparent while inside Hero.

Blur background only after scrolling.

Height

72px desktop

64px tablet

56px mobile

Items

Think

Build

Learn

Explore

Connect

Language

Theme

Resume

GitHub

LinkedIn

Navigation should feel almost invisible.

---

# Hero Portrait

Purpose

Introduce the human behind the work.

Not a corporate profile photo.

Not a LinkedIn picture.

The portrait becomes part of the composition.

---

## Asset Specification

Filename

hero-portrait.webp

Transparent background

Required

Minimum height

2200 px

Lighting

Soft

Natural

No hard shadows

Expression

Relaxed

Curious

Professional

Wardrobe

Neutral colors

No visible logos

No distracting accessories

Pose

Body slightly turned toward the center.

Eyes looking near the content.

Not directly into the camera.

Hair should preserve natural texture.

Avoid aggressive editing.

---

# Portrait Integration

The portrait should blend with the interface.

No visible rectangular boundaries.

Edges softly fade into the background.

The image appears to emerge from the workspace.

Never like a pasted photograph.

---

# Headline

Maximum

2 lines

Target reading time

2 seconds

The headline should communicate mindset.

Not profession.

Typography

Largest on the page.

Approximate width

45–55% of the layout.

---

# Supporting Text

Maximum

4 lines

Readable in under 15 seconds.

Tone

Human.

Reflective.

Honest.

No buzzwords.

No marketing language.

---

# Primary Action

Label

Explore

Purpose

Continue the experience.

Never:

"Learn More"

"Read More"

"Discover"

The visitor is already exploring.

---

# Secondary Actions

Resume

GitHub

LinkedIn

These actions remain visually quieter.

The experience itself remains primary.

---

# Three.js Scene

Purpose

Represent thinking.

Not technology.

---

## Objects

Nodes

Represent ideas.

Connections

Represent relationships.

Groups

Represent domains of knowledge.

Movement

Represents continuous refinement.

---

## Rules

No floating particles.

No random geometry.

No decorative motion.

Every node belongs to the system.

Objects reorganize slowly.

Connections evolve naturally.

Nothing suddenly appears.

Nothing disappears without reason.

---

# Mouse Interaction

Mouse movement gently influences nearby nodes.

Objects react with slight inertia.

Maximum displacement

20 px

No exaggerated parallax.

No dramatic reactions.

The visitor should almost wonder whether the movement is intentional.

---

# Camera

Static by default.

Very subtle depth.

During scroll

Camera slowly advances.

Never rotates.

Never spins.

Never tilts dramatically.

Movement should resemble walking toward a workspace.

---

# Scroll Transition

As the visitor scrolls

The network becomes denser.

Connections become clearer.

The portrait gradually integrates with the background.

Attention naturally shifts toward Think.

The visitor should never perceive a page change.

Only progression.

---

# Background

Light Mode

Soft neutral gradient.

Almost imperceptible.

Dark Mode

Warm charcoal.

Subtle depth.

No visible textures competing with content.

---

# Motion

Portrait

Soft fade + slight upward movement.

Headline

Fade with minimal vertical offset.

Supporting text

Appears after headline.

Buttons

Appear last.

Three.js

Already alive before everything else.

It should feel like the environment existed before the visitor arrived.

---

# Accessibility

Everything remains readable with JavaScript disabled.

The canvas never blocks interaction.

Portrait includes descriptive alt text.

Keyboard navigation reaches every interactive element.

Reduced-motion users receive a simplified version.

---

# Performance

Hero should render immediately.

Three.js initializes after primary content becomes visible.

Prioritize text.

Then portrait.

Then WebGL.

---

# Mobile

Portrait appears above content.

Three.js complexity reduced by approximately 60%.

Navigation collapses.

Text width increases.

Buttons stack vertically.

Reading always remains the priority.

---

# Required Assets

hero-portrait.webp

hero-background-gradient.svg (optional)

node-texture.webp

resume-en.pdf

resume-es.pdf

favicon

social-icons.svg

---

# Developer Notes

This screen defines the emotional tone of the entire portfolio.

Do not attempt to impress.

Attempt to create confidence.

The interface should feel crafted.

Quiet.

Thoughtful.

Every pixel should suggest that someone cared about every decision.
