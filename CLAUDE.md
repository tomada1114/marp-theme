# CLAUDE.md

This file provides guidance to Claude Code when working with this repository.

## Project Overview

Marp theme collection for YouTube recording slides. Contains CSS themes and the `marp-slide-writer` skill for creating presentation slides.

## Quick Reference

| Task | Command |
|------|---------|
| Preview slides | `npx @marp-team/marp-cli slides/slides.md --html --preview --watch` |
| Validate slides | `python .claude/skills/marp-slide-writer/scripts/validate_slides.py slides/slides.md` |

## Directory Structure

```
marp-theme/
├── youtube-theme.css                    # Main theme (GitHub Pages)
├── CLAUDE.md                            # This file
├── README.md                            # Theme documentation
└── .claude/
    └── skills/
        └── marp-slide-writer/           # Slide writing skill
            ├── SKILL.md                 # Skill definition
            ├── reference.md             # Layout constraints
            ├── templates/               # Slide templates
            ├── examples/                # Example slides
            └── scripts/                 # Validation scripts
```

## Theme URL

```
https://tomada1114.github.io/marp-theme/youtube-theme.css
```

## Skill Activation Rules

When the user mentions the following keywords, ALWAYS use the Skill tool:

| Keywords | Skill |
|----------|-------|
| スライド作成, Marp, プレゼン資料, 収録用スライド, presentation | `marp-slide-writer` |

## CSS Development

When modifying `youtube-theme.css`:

1. Test changes with live preview
2. Verify all CSS classes still work
3. Check layout constraints are maintained
4. Push to main branch (GitHub Pages auto-deploys)

## Slides Workflow

1. Create slide file from template
2. Edit content following layout constraints
3. Validate with `validate_slides.py`
4. Preview with Marp CLI
5. Fix any violations before finalizing
