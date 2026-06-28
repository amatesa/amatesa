# 04 — Design System

## Project

Personal Portfolio Website

Version 1.0

---

# Design Philosophy

The interface should disappear.

The visitor should focus on ideas, projects and interactions rather than the interface itself.

Visual design exists to organize information, create rhythm and encourage exploration.

Every component should feel intentional.

---

# Design Principles

Clarity before decoration.

Consistency before originality.

Interaction before animation.

Whitespace before density.

Content before interface.

Motion before effects.

---

# Visual Density

Low.

Every screen should breathe.

Avoid visual noise.

Avoid crowded layouts.

Each section should contain one primary focus.

---

# Grid System

Desktop

12-column grid

Max content width:

1280px

Content width:

1120px

Large sections may exceed this only for photography or immersive layouts.

Tablet

8-column grid

Mobile

4-column grid

---

# Spacing Scale

Base Unit

8px

Spacing Tokens

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

Never use arbitrary spacing.

---

# Border Radius

Small

8px

Medium

16px

Large

24px

Extra Large

32px

Never use perfectly square cards.

Never use exaggerated rounded corners.

---

# Shadows

Very soft.

Large blur.

Low opacity.

Shadow exists only to separate layers.

Never for decoration.

---

# Elevation

Level 0

Background

Level 1

Cards

Level 2

Expanded cards

Level 3

Dialogs

Level 4

Navigation

Maximum four elevation levels.

---

# Color Tokens

Primary

#174349

Primary Hover

Automatically generated

Primary Active

Automatically generated

Surface Light

Neutral

Surface Dark

Neutral

Text Primary

Near Black

Text Secondary

Gray

Text Disabled

Light Gray

Borders

Subtle

Success

Muted Green

Warning

Muted Amber

Error

Muted Red

Never use saturated colors.

---

# Theme Rules

Light mode and Dark mode are separate systems.

Never invert colors automatically.

Each theme should be manually tuned.

Dark mode should preserve depth.

Light mode should preserve softness.

---

# Typography

Primary Font

Inter

Fallback

Manrope

Fallback

System UI

---

# Type Scale

Display

64

H1

48

H2

36

H3

28

H4

22

Body Large

20

Body

18

Body Small

16

Caption

14

Mobile sizes should scale proportionally.

---

# Font Weights

400

500

600

700

Avoid using many different weights.

---

# Paragraph Width

Maximum

70 characters

Readable text is more important than filling space.

---

# Buttons

Primary

Filled

Secondary

Outline

Tertiary

Text

Ghost

Transparent

Icon Button

Minimal

Every button should have:

Hover

Focus

Pressed

Disabled

Loading

---

# Cards

Cards are not boxes.

Cards are content containers.

Large padding.

Soft edges.

Clear hierarchy.

Every card should have an interactive state.

---

# Images

Use WebP whenever possible.

Lazy loading.

Rounded corners only when appropriate.

Photography should blend naturally with backgrounds.

Never place a floating rectangular image on screen.

---

# Icons

SVG only.

Consistent stroke.

24px default.

20px on mobile.

No icon fonts.

---

# Lists

Never use long bullet lists.

Prefer grouped information.

Prefer visual hierarchy.

---

# Dividers

Very subtle.

Used only when necessary.

Whitespace is preferred.

---

# Forms

Minimal.

One column.

Large inputs.

Clear labels.

Accessible focus.

Immediate validation.

---

# Navigation

Sticky.

Transparent initially.

Solid after scrolling.

Height

72px

Desktop

64px

Mobile

Logo area

Navigation

Theme

Language

Resume

---

# Scroll Behavior

Smooth.

Never exaggerated.

Anchor navigation.

Respect reduced motion settings.

---

# Section Rhythm

Each section should occupy approximately one viewport height.

Some sections may exceed one screen when content requires it.

Never force scrolling simply to fit a design.

---

# Visual Balance

Every screen should contain:

One dominant element.

One supporting element.

One action.

Nothing more.

---

# Component States

Default

Hover

Focus

Active

Disabled

Loading

Empty

Every reusable component must define all states.

---

# Responsive Rules

Desktop is redesigned.

Tablet is redesigned.

Mobile is redesigned.

Layouts are never simply compressed.

Content priority changes.

Typography scales.

Spacing adapts.

Interactions remain consistent.

---

# Motion Budget

Maximum animation duration

600ms

Preferred

250–400ms

Micro interactions

150–250ms

Avoid long animations.

Visitors should never wait for the interface.

---

# Accessibility

Minimum contrast

WCAG AA

Preferred

AAA whenever possible

Keyboard navigation

Complete

Screen readers

Supported

Focus visible

Always

Reduced Motion

Fully supported

---

# Performance

Lighthouse

95+

Largest Contentful Paint

Under 2 seconds

Minimal JavaScript

Minimal CSS

No unnecessary libraries.

---

# Reusability

Every section is built from reusable components.

No duplicated layouts.

No duplicated styling.

No duplicated interactions.

---

# Final Principle

The design should never compete with the content.

If a visitor remembers the animations more than the projects, the design has failed.

If a visitor remembers how naturally the experience flowed, the design has succeeded.
