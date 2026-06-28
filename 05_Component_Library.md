# 05 — Component Library

## Project

Personal Portfolio Website

Version 1.0

---

# Objective

Every interface element must be reusable.

No component should be designed specifically for a single page.

Every component must support both Light and Dark themes.

Every component must be fully responsive.

---

# Component Hierarchy

Layout Components

↓

Section Components

↓

Content Components

↓

Interactive Components

↓

Utility Components

---

# Layout Components

## Page

Defines the global page structure.

Contains:

Navigation

Main Content

Footer

No business logic.

---

## Container

Defines maximum content width.

Centered.

Responsive.

Never contains visual styling.

---

## Section

Reusable content block.

Every section supports:

Background

Padding

Anchor

Animation

Section ID

Optional divider

---

# Navigation

Sticky.

Transparent at top.

Solid after scroll.

Contains:

Logo / Name

Navigation

Language

Theme

Resume

Mobile Menu

Behavior

Desktop

Horizontal.

Mobile

Drawer.

Never full-screen.

---

# Hero

Purpose

Immediately communicate identity.

Contains

Portrait

Headline

Short Statement

Primary CTA

Secondary CTA

Optional Background Layer

Portrait behavior

Soft mask.

Integrated into background.

Never framed.

Never circular.

---

# Section Header

Reusable.

Contains

Eyebrow

Title

Subtitle

Optional Action

Always left aligned.

---

# Process Diagram

Interactive component.

Represents:

Understand

↓

Analyze

↓

Break Down

↓

Build

↓

Improve

↓

Repeat

Each node expands.

Connections animate.

No modal windows.

---

# Project Module

Core component.

Contains

Project Cover

Title

Problem

Approach

Outcome

Lessons

Technologies

Links

Optional Gallery

Optional Demo

Optional Repository

Supports

Collapsed

Expanded

Fullscreen

---

# Project Gallery

Responsive grid.

Supports

Images

Videos

GIF

Embedded YouTube

Image comparison

Lazy loading.

---

# Timeline

Vertical.

Desktop.

Horizontal scrolling on mobile.

Supports

Date

Title

Description

Icon

Optional Image

---

# Learning Card

Used inside Learn section.

Contains

Institution

Title

Description

Skills

Status

Completed

In Progress

Planned

---

# Skill Chip

Minimal.

Interactive.

Hover reveals description.

Never decorative.

Categories

Data

Development

Games

AI

Operations

Design

---

# Technology Stack

Grouped.

Never alphabetical.

Displayed by category.

Optional section.

Can be disabled through configuration.

---

# Repository Card

GitHub integration.

Contains

Repository Name

Description

Language

Updated Date

Topics

Repository Link

Pinned indicator

Optional statistics.

---

# Resource Card

Used for:

Books

Articles

Talks

Future content

Can remain hidden until enabled.

---

# CTA Block

Reusable.

Contains

Short message

Primary button

Secondary button

Used before Contact section.

---

# Contact Card

Contains

LinkedIn

GitHub

Email

Itch.io

Resume

Icons only support.

Text remains primary.

---

# Footer

Minimal.

Contains

Copyright

Current Year

Portfolio Version

Built by Alejandro

Optional GitHub Link

---

# Button System

Primary

Secondary

Ghost

Text

Icon

Every button supports

Hover

Focus

Pressed

Disabled

Loading

Success

---

# Modal

Avoid when possible.

Prefer expanding content inline.

Only use for

Image Viewer

Video Viewer

Large Preview

---

# Tooltip

Simple.

Short.

Maximum two lines.

Never required to understand content.

---

# Accordion

Used only when information density requires it.

Default state

Collapsed.

---

# Tabs

Allowed only for

Language

Project Variants

Gallery Categories

Never use tabs for navigation.

---

# Tags

Small.

Minimal.

Used for

Technology

Category

Status

Role

---

# Notification

Reserved for future use.

Currently disabled.

---

# Loading States

Every asynchronous component supports

Skeleton

Spinner

Placeholder

Avoid blank areas.

---

# Empty States

Every optional section must define

Empty illustration

Short message

Suggested action

---

# Image Placeholder

Every image component supports placeholder assets.

Placeholder ratio remains identical to final image.

Replacing images must never require layout changes.

---

# Configurable Sections

Every major section can be enabled or disabled through a configuration file.

Think

Build

Learn

Explore

Connect

Timeline

Technologies

Books

Writing

Experiments

Blog

Open Source

Future Projects

Disabling a section must never break spacing or navigation.

---

# Animation Hooks

Every component exposes animation hooks.

Enter

Exit

Hover

Focus

Expanded

Collapsed

Animations are defined separately.

Components never contain animation logic.

---

# Accessibility

Every component supports

Keyboard navigation

ARIA labels

Visible focus

Reduced motion

Screen readers

---

# Component Rule

If two components solve the same problem,

merge them.

If one component needs many exceptions,

split it.

Consistency is more important than quantity.

---

# Final Principle

The interface should feel like a coherent system.

Not a collection of independent widgets.

Every component should look as if it belongs to the same product.
