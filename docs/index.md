---
title: "Gastown GUI — Web Dashboard"
description: "Web interface for the Gastown multi-agent orchestrator. Real-time monitoring, service control, and work visualization."
date: 2026-04-13
---

# Gastown GUI

Web dashboard companion for Gastown. Vanilla JS SPA + Express server wrapping the `gt` CLI.

## Features

- Real-time event stream from `gt feed --json` via WebSocket
- Service control panel (Mayor, Deacon, Witness, Refinery)
- Agent state visualization
- Beads/convoy tracking

## Architecture

| Layer | Technology |
|-------|-----------|
| Server | Express.js (monolith, partially refactored into modules) |
| Client | Vanilla JS (no framework, no build step) |
| Communication | WebSocket for real-time events |
| Port | 7667 (configurable via GASTOWN_PORT) |

## Planning & Specs

Full specifications at [plan/gastown-gui/](https://github.com/getHarshOnline/plan/tree/main/gastown-gui).
