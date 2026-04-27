<p align="center">
  <img src="docs/images/logo.png" width="400" alt="VibeClaw Workbench Logo">
</p>

<p align="center">
  <b>VibeClaw Workbench</b><br>
  High-performance local tool management and context switching interface for multi-environment orchestration.
</p>

<p align="center">
  <a href="#overview">Overview</a> •
  <a href="#features">Features</a> •
  <a href="#use-cases">Use Cases</a> •
  <a href="#evidence">Evidence</a> •
  <a href="#setup">Setup</a>
</p>

---

## Overview
**VibeClaw Workbench** is a professional environment orchestration platform designed for senior engineers. It provides a forensic-grade interface for managing isolated local development workspaces, allowing for seamless context switching without environment drift or dependency conflicts.

## Features
- **Project Indexing**: Automated recursive scanning and manifest hashing of all local repositories.
- **Context Isolation**: Forensic-grade management of environment variables to prevent context leakage.
- **Auto-Recovery**: Integrated path-repair logic for broken workspace links and restricted directories.
- **Vibe Orchestration**: One-command activation of project-specific technical stacks and logic cores.

## Use Cases
- **Multi-Repo Management**: Orchestrate 10+ isolated projects from a single forensic dashboard.
- **Context Preservation**: Switch between divergent tech stacks (e.g., Rust to Python) with zero variable residue.
- **Legacy Path Repair**: Automatically identify and relink workspace directories after system rearrangement.

## Evidence: Tool in Action
<p align="center">
  <img src="VibeClaw/demo/showcase.png" width="600" alt="VibeClaw Workbench Showcase">
  <br>
  <i>Figure 1: Automated environment scan identifying and indexing 8 active workspaces.</i>
</p>

## Setup
1. **Initialize**: Define your workspace root in the primary config.
2. **Scan**: Run `python VibeClaw-Workbench.py --scan` to index your technical vault.
3. **Switch**: Use the activation command to load your project-specific "vibe."

## Safety
A local-only orchestration layer. Your directory structures and environment variables are never shared externally.
