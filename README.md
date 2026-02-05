# Character Forge

Character Forge is a web-based character creator and Progressive Web App (PWA) that allows users to visually assemble a character using modular parts (body, face, hair, eyes, etc.) and then generate a high-detail AI-rendered version using an external image generation API.

The system follows a **template-first, AI-second** approach to ensure consistency, control, and repeatability.

---

## Overview
Most AI image generators lack precise control over character identity. Character Forge solves this by separating **structure** from **creativity**.

Users build a character visually.  
AI enhances it without redefining it.

---

## Core Concept
- Modular character construction
- Deterministic character blueprint (JSON)
- System-enforced prompt structure
- User-driven creative prompting
- AI used as a renderer, not a designer

---

## Target Users
- Game developers
- Writers & worldbuilders
- RPG / tabletop players
- Creative hobbyists

---

## Features

### MVP
- Modular 2D character builder
- Live template preview
- User text prompt input
- AI image generation
- Template lock (hard / soft)
- PWA support

### Phase 2
- Presets & archetypes
- Multiple art styles
- Save / load characters
- Export options

---

## Art Styles

Character Forge is designed to support multiple visual styles through template locking and prompt control.

### Initial Focus
- **Anime-style characters** (primary MVP focus)

### Planned
- Cartoon 2D
- Flat illustration
- Pixel art
- Semi-realistic illustration

Photorealistic and 3D styles are explicitly out of scope.

---

## Tech Stack
- **Frontend**: React, TypeScript, Vite, Tailwind CSS
- **State**: Zustand
- **Backend**: Node.js, Express, TypeScript
- **AI**: Perchance Image Generation API
- **PWA**: Workbox
- **Hosting**: Vercel / Netlify (frontend), Railway / Fly.io (backend)

---

## High-Level Architecture
1. User assembles character template
2. System generates character blueprint
3. Prompt composer merges:
   - system rules
   - template description
   - style lock
   - user prompt
4. Backend invokes AI API
5. Final image is returned

---

## Status
🚧 Early architecture & planning phase
