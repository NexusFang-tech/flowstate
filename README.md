# FLOWSTATE — Automation Workflow Builder

Visual drag-and-drop automation workflow builder. Design automation flows with 16 node types, conditional branching, loops, delays, and output actions. Includes 4 pre-built workflow templates and exports to JSON, pseudocode, Mermaid diagrams, and Power Automate-style definitions. Single HTML file, zero dependencies.

## Live Demo

**[nexusfang-tech.github.io/flowstate](https://nexusfang-tech.github.io/flowstate/)**

## Node Types (16)

| Category | Nodes |
|----------|-------|
| Triggers | Schedule (cron), Webhook (HTTP), Event (system), Manual |
| Actions | HTTP Request, Send Email, Teams Message, Database Query, Transform Data, Run Script |
| Logic | If/Else (conditional branch with Yes/No ports), Switch (multi-path) |
| Flow Control | Delay/Wait, For Each (loop) |
| Outputs | Log Output, Write File |

## Features

- **Drag-and-drop canvas** — Drag nodes from the palette, place anywhere on an infinite canvas
- **Visual connections** — Click output ports and drag to input ports to create bezier curve links. Condition nodes have separate Yes/No output ports with color coding (green/pink)
- **Node configuration** — Click any node to edit in the properties panel with type-appropriate inputs (HTTP method dropdowns, code textareas, cron expressions, etc.)
- **Conditional branching** — If/Else nodes with separate Yes and No output paths
- **4 pre-built templates**:
  - Employee Onboarding (M365 / Graph API)
  - Security Alert Pipeline (SIEM → triage → route)
  - Backup Verification (schedule → check → alert)
  - Helpdesk Ticket Flow (form → categorize → assign → notify)
- **Validation engine** — Checks for missing triggers, orphan nodes, dead ends, and incomplete configurations
- **Undo/Redo** — Full state history (Ctrl+Z / Ctrl+Y)
- **Auto layout** — BFS-based left-to-right arrangement
- **Save/Load** — Browser localStorage persistence
- **Minimap** — Overview with node positions

## Export Formats

| Format | Description |
|--------|-------------|
| JSON | Full workflow definition, re-importable |
| Pseudocode | Human-readable logic with IF/ELSE/FOR blocks |
| Mermaid | Diagram markup for embedding in documentation |
| Power Automate | Conceptual trigger/action definition matching PA structure |

## Tech Stack

Vanilla JavaScript · HTML Canvas · CSS · GitHub Pages

## Author

**Matt Keith** · [nexusfang-tech.github.io](https://nexusfang-tech.github.io)
