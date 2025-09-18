# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Vue 3 presentation application showcasing Claude Code features. The app uses a slide-based navigation system with keyboard controls, mouse wheel support, and theme switching.

## Commands

```bash
# Development
npm run dev          # Start Vite dev server on port 8080

# Build
npm run build        # Build for production

# Preview
npm run preview      # Preview production build
```

## Architecture

### Core Structure

- **Main Entry**: `src/main.js` mounts the `PresentationSlider` component
- **Slide System**: `src/components/PresentationSlider.vue` manages slide navigation, keyboard/mouse controls, and theme switching
- **Individual Slides**: Located in `src/components/slides/` directory, each slide is a separate Vue component

### Key Features

1. **Navigation**: Arrow keys, Page Up/Down, Space bar, and mouse wheel for slide navigation
2. **Theme Switching**: Dark/light mode toggle with localStorage persistence
3. **Slide Memory**: Current slide position saved to localStorage
4. **Transitions**: Custom slide transitions with opacity and direction animations

### Technology Stack

- **Vue 3**: Composition API with `<script setup>` syntax
- **Vite**: Build tool and dev server
- **Tailwind CSS**: Utility-first styling with dark mode support
- **PostCSS**: CSS processing with nested rules support
- **Heroicons**: Icon components for UI elements

### Style Guide

#### Links
- Use `text-cyan-400 hover:text-cyan-300` for all links
- All external links must include `target="_blank"`
- Format: `<a href="URL" target="_blank" class="text-cyan-400 hover:text-cyan-300">Link Text</a>`
- Normal links: default text size
- Source/reference links: add `text-xs` class
- Block links: add `block` class for vertical stacking
- Use `<span class="opacity-40">|</span>` between inline navigation links

##### Link Examples
```html
<!-- Standard link -->
<a href="https://example.com" target="_blank" class="text-cyan-400 hover:text-cyan-300">Example</a>

<!-- Small source link -->
<a href="source.com" target="_blank" class="text-cyan-400 hover:text-cyan-300 text-xs">→ Read more</a>

<!-- Navigation bar -->
<a href="#" class="text-cyan-400 hover:text-cyan-300">Link 1</a>
<span class="opacity-40">|</span>
<a href="#" class="text-cyan-400 hover:text-cyan-300">Link 2</a>
```

#### Code Blocks
- Use `code-block` class for container
- Add `opacity-60` label above code
- Use `<span class="opacity-60">` for comments

#### Cards
- Use `card rounded-lg p-6` for consistent card styling
- Headers: `text-lg font-semibold mb-3` for card titles
- Code block headers: `text-xl font-semibold mb-4`

#### Slide Structure
1. Always wrap in `<div class="slide absolute inset-0">`
2. Center content with `flex items-center justify-center min-h-screen p-8`
3. Max width container: `max-w-6xl w-full`
4. Title: `text-3xl font-bold mb-6 text-center gradient-text`
5. Subtitle: `text-center opacity-80 mb-12 max-w-2xl mx-auto`

### Slide Components

All slides follow a consistent pattern with `.slide` class wrapper and use Tailwind utilities for styling. The presentation covers:

- Memory system
- Slash commands
- Subagents
- GitHub integration
- Tools/MCP
- Best practices
- Roadmap
- ACP (Anthropic Claude Platform)
- Competitive analysis
- Business analysis
- Product Manager use cases
- Business Analyst use cases
- CTO use cases
- Marketing Manager use cases
- QA Engineer use cases
- Custom MCP
- Context engineering
