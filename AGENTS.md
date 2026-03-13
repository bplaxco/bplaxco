# AGENTS.md

This file provides guidance to AI agents when working with code in this repository.

## Repository Overview

This is a personal repository containing:
- Personal work style and communication preferences (README.md)
- A workflow diagram visualizing task triage and execution process (workflow/)

## Building the Workflow Diagram

The workflow diagram is created using D2 (a modern diagram scripting language).

**Build the diagram:**
```bash
cd workflow
make
```

**Watch for changes and auto-rebuild:**
```bash
cd workflow
make watch
```

Requirements: `make`, `d2`, and optionally `inotifywait` for watch mode.

## Working with the Workflow

- **Source file:** `workflow/workflow.d2` - Edit this file to modify the workflow diagram
- **Output file:** `workflow/workflow.svg` - Generated SVG diagram (don't edit directly)
- The workflow uses the ELK layout engine and includes custom classes for styling different node types (decision, terminal, storage, action, critical)
