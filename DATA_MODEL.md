# Character Blueprint Data Model

## Schema (v1)

{
  "body": "slim | athletic | heavy",
  "face": "oval | square | round",
  "eyes": {
    "shape": "almond | round | narrow",
    "iris": "color"
  },
  "hair": {
    "style": "short | long | tied",
    "color": "color"
  },
  "nose": "small | sharp | wide",
  "mouth": "neutral | smile | stern",
  "hands": "normal | slender | armored",
  "feet": "bare | boots | shoes",
  "style": "fantasy | anime | cartoon"
}

## Style Enforcement

The `style` field controls:
- Allowed asset sets
- Prompt vocabulary
- Template lock strength

Example:
"style": "anime"

## Constraints
- Fixed proportions per body type
- No dynamic resizing in MVP
- Schema must be versioned
