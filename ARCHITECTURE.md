# Architecture

## System Overview
Character Forge uses a template-first pipeline where character structure is defined before AI generation.

## Major Components
- Character Builder UI
- Character Blueprint Generator
- Prompt Composer
- AI Rendering Service

## Data Flow
User → Template Builder → Blueprint → Prompt Composer → AI API → Final Image
