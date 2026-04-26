---
name: voice
description: Configure the preferred reframe voice for the second-arrow skill. Set a specific voice, random/contextual mode, or reset to the picker experience.
license: MIT
metadata:
  author: second-arrow
  version: "1.0"
---

# /voice — Configure Reframe Voice

## What this command does

Sets or clears the preferred voice used when the second-arrow skill fires a reframe. If a voice is set, reframes skip the picker and rewrite directly in that voice.

## Operations

### `/voice` (no args)

Show current configuration and all available voices. Prompt the user to pick one.

Display:
```
Current voice: [voice name] | not configured (picker will appear on next reframe)

Available voices:
○ Carnegie   — friendly & practical
○ Stoic      — cool & precise
○ Daoist     — soft & indirect
○ Confucian  — names the reciprocity directly
○ Second Arrow — separates the real frustration from the added layer
○ Metta      — warm & steady
○ Askell     — names what this pattern does to the work
○ random     — contextual default chosen per trigger type

Run /voice <name> to set. Run /voice reset to return to the picker.
```

### `/voice <name>`

Set the preferred voice. Voice names are case-insensitive.

Valid names: `carnegie`, `stoic`, `daoist`, `confucian`, `second-arrow`, `metta`, `askell`, `random`

Save to Claude's memory:
> Preferred second-arrow reframe voice: [name]

Confirm to user:
> Voice set to **[Name]**. Reframes will use this voice going forward. Run `/voice reset` to return to the picker.

### `/voice random`

Sets contextual mode. Claude picks per trigger type using the Voice defaults table — no fixed preference.

Save to memory:
> Preferred second-arrow reframe voice: random

Confirm:
> Voice set to **random**. Claude will pick contextually for each reframe (self-hostile → Second Arrow, hostility → Carnegie, drift → Stoic).

### `/voice reset`

Clears the stored preference. Returns to the unconfigured picker experience.

Remove from memory:
> Preferred second-arrow reframe voice: [remove entry]

Confirm:
> Voice preference cleared. The picker will appear on the next reframe.

## Error handling

Unrecognized name:
> "[name]" isn't a valid voice. Valid options: `carnegie`, `stoic`, `daoist`, `confucian`, `second-arrow`, `metta`, `askell`, `random`
