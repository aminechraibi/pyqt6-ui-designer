# PyQt6 UI Designer Skill

A Claude Code skill for designing and refining modern, professional PyQt6 desktop interfaces using a consistent visual system, light/dark themes, and production-ready QSS.

## Quick start

Trigger the skill in Claude Code by invoking it directly for a new UI or an existing codebase refresh:

```text
/pyqt6-ui-designer Generate a professional app shell with cards and navigation.
```

Other example tasks supported by the skill:

- "Make this PyQt6 window look modern."
- "Add a dark mode sidebar."
- "Refine this table and toolbar."
- "Style my buttons and inputs consistently."

## What it does

The skill acts as a PyQt6 UI design assistant that enforces an enterprise design system across generated code. It focuses on:

- **Token-based design**: Uses canonical colors, typography, spacing, and elevation from `references/design_tokens.md`.
- **4px spacing discipline**: Enforces a strict 4px grid for all layouts without magic numbers.
- **Theme parity**: Generates both light and dark variants with all interactive states (default, hover, pressed, focus, disabled).
- **Component reuse**: Applies proven QSS patterns and templates for sidebars, tables, modals, and forms from `references/component_library.md` and `references/qss_patterns.md`.
- **API accuracy**: Uses Context7 MCP lookups to verify PyQt6 properties, QSS pseudo-state selectors, and layout managers.

## Included structure

```text
SKILL.md
references/
├── component_library.md
├── design_tokens.md
└── qss_patterns.md
```

## Installation

To use this skill in your Claude Code projects:

1. Create a `.claude/skills/pyqt6-ui-designer/` directory in your project root.
2. Copy `SKILL.md` and the `references/` folder into that directory.
3. When you open Claude Code, the `/pyqt6-ui-designer` skill will automatically be available.
