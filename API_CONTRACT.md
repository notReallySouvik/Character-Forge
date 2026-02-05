# API Contract

## POST /generate

### Input
{
  "characterBlueprint": { ... },
  "userPrompt": "string",
  "lockStrength": "hard | soft"
}

### Output
{
  "imageUrl": "string",
  "metadata": { }
}

### Errors
- 400 Invalid blueprint
- 500 AI generation failed
