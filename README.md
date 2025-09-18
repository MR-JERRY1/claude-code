# Claude Code Presentation

An interactive presentation showcasing Claude Code features and capabilities, built with Vue 3 and Vite.

## Overview

This is a slide-based presentation application that demonstrates Claude Code's features including memory system, slash commands, subagents, GitHub integration, and various use cases across different roles.

## Features

- **Interactive Navigation**: Navigate slides using keyboard (arrow keys, space, page up/down) or mouse wheel
- **Dark/Light Theme**: Toggle between dark and light modes with persistent preference
- **Slide Memory**: Automatically remembers your current slide position
- **Smooth Transitions**: Custom slide transitions with directional animations
- **Responsive Design**: Optimized for various screen sizes

## Quick Start

### Prerequisites

- Node.js (v14 or higher)
- npm or yarn

### Installation

```bash
# Clone the repository
git clone <repository-url>
cd claude-code

# Install dependencies
npm install
```

### Development

```bash
# Start development server on port 8080
npm run dev
```

### Production Build

```bash
# Build for production
npm run build

# Preview production build
npm run preview
```

## Project Structure

```bash
claude-code/
├── src/
│   ├── main.js              # Application entry point
│   ├── style.css            # Global styles and Tailwind imports
│   ├── components/
│   │   ├── PresentationSlider.vue  # Main slider controller
│   │   └── slides/          # Individual slide components
│   │       ├── Slide1.vue   # Title slide
│   │       ├── Slide2.vue   # Memory system
│   │       └── ...          # Additional slides
│   └── assets/              # Static assets
├── index.html               # HTML entry point
├── package.json            # Dependencies and scripts
├── vite.config.js          # Vite configuration
├── tailwind.config.js      # Tailwind CSS configuration
└── CLAUDE.md              # Project guidelines for Claude Code
```

## Navigation Controls

| Action | Keys |
|--------|------|
| Next Slide | Right Arrow, Space, Page Down |
| Previous Slide | Left Arrow, Page Up |
| Toggle Theme | Click theme icon in top-right |
| Mouse Wheel | Scroll to navigate slides |

## Technology Stack

- **Vue 3**: Progressive JavaScript framework with Composition API
- **Vite**: Next-generation frontend tooling
- **Tailwind CSS**: Utility-first CSS framework with dark mode support
- **Heroicons**: Beautiful hand-crafted SVG icons
- **PostCSS**: CSS processing with nested rules support

## Slide Topics

The presentation covers the following Claude Code features:

1. **Introduction**: Welcome and overview
2. **Memory System**: How Claude Code maintains context
3. **Slash Commands**: Quick actions and productivity tools
4. **Subagents**: Specialized task delegation
5. **GitHub Integration**: Seamless version control
6. **Tools & MCP**: Model Context Protocol and tool ecosystem
7. **Best Practices**: Tips for effective usage
8. **Roadmap**: Future developments
9. **ACP**: Anthropic Claude Platform
10. **Use Cases**: Role-specific demonstrations for:
    - Product Managers
    - Business Analysts
    - CTOs
    - Marketing Managers
    - QA Engineers
11. **Custom MCP**: Building custom integrations
12. **Context Engineering**: Advanced prompt optimization

## Development Guidelines

See [CLAUDE.md](./CLAUDE.md) for detailed development guidelines and code style conventions.