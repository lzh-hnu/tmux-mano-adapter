# tmux for Mano: Long-Horizon Terminal Adapter

## Purpose

This document records the research framing behind the static GitHub Pages site. The project studies how tmux can be adapted for Mano as a durable terminal substrate for agentic work.

## Research Question

How should Mano use tmux to plan, pause, resume, and audit long-running shell workflows?

## Working Thesis

The adapter gives Mano a durable execution substrate where panes represent planning lanes, observation surfaces, and rollback anchors.

## Design Claims

- Long-running commands receive explicit lifecycle annotations.
- Window and pane layout encode planning structure rather than incidental display state.
- Interruption handling records what changed before, during, and after recovery.

## Evaluation Lens

- Long-horizon continuity
- Interruption recovery
- Audit completeness for delayed outcomes


## Threats to Validity

- Terminal state can be over-instrumented, causing an adapter to measure artifacts of the harness rather than real agent behavior.
- A final successful artifact may hide poor recovery behavior, repeated command attempts, or fragile focus management.
- Agent-specific adapters can become difficult to compare unless trace schemas remain explicit and documented.

## Hero Image Source

The GitHub Pages hero image uses a 700x500 version of the shared tmux CUA screenshot, copied into `docs/assets/hero.png` and displayed below the page title at its native size.
