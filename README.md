# skills (demo repo)

This repo is a **demo skills repo** organized into **two top-level roots** (think: two different agents/products), each with its own `skills/` directory.

It follows the conventions described in the upstream `SKILL.md` spec:
- Each skill lives in `skills/<skill-name>/SKILL.md`
- `SKILL.md` begins with YAML frontmatter that supports **only** `name` and `description`
  - `name`: letters/numbers/hyphens only
  - `description`: **starts with "Use when..."** and describes triggering conditions only (not workflow)

## Structure

```
assistant-a/
  skills/
    writing-email-subjects/
      SKILL.md
    writing-meeting-notes/
      SKILL.md
assistant-b/
  skills/
    triaging-bugs/
      SKILL.md
    writing-release-notes/
      SKILL.md
```

## Adding a new skill

1. Create a folder under one of:
   - `assistant-a/skills/<skill-name>/`
   - `assistant-b/skills/<skill-name>/`
2. Add `SKILL.md` with:
   - YAML frontmatter containing only `name` and `description`
   - Body sections like: Overview, When to Use, Quick Reference, Implementation, Common Mistakes
