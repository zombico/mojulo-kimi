# Mojulo × Kimi Code

Thin Kimi Code adapter for **Mojulo 3.0.0**, the deterministic 3D compiler for coding agents.

This repository contains no Mojulo renderer/runtime fork. It teaches Kimi Code how to bootstrap and operate the published `mojulo` npm package inside the active workspace.

## Architecture

```text
Kimi Code
   |
Kimi plugin
   |
Mojulo skill
   |
workspace-local mojulo@3.0.0
   |
recipes / refs / checkpoints / exports
```

## Install

Inside Kimi Code:

```text
/plugins install https://github.com/zombico/mojulo-kimi
```

Then run `/reload` or start a new session.

## Example

> Build a procedural modern 3D city with varied building heights, a clear street layout, landmark towers and surrounding terrain. Then edit the same city to make downtown denser and export GLB + HTML.

## Design rule

The adapter owns agent instructions and bootstrap only.

Mojulo core owns geometry, recipes, editing, exporters, checkpointing and deterministic state.

## Requirements

- Node.js >= 22.14
- npm access
- writable workspace

## Project status

Initial Kimi adapter scaffold for Mojulo 3.0.0.
