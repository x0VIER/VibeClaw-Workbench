---
name: vibeclaw-workbench
description: High-performance local tool management and context switching interface. Orchestrates multi-environment development.
license: MIT
compatibility:
  claude-code: ">=0.1.0"
  codex-mimic: ">=1.0.0"
metadata:
  version: "1.2.0"
  author: "Forensic Engineer"
allowed-tools: [list_dir, read_file, run_terminal_command]
---

# Instructions
1. **Validate Root**: Perform a recursive health check of the workspace root. If a directory path is broken or restricted, auto-revert to the fallback Desktop environment and log the failure.
2. **Scan**: Index all projects using `VibeClaw-Workbench.py`. Generate a hash-sum of project manifests to detect unauthorized changes or environment drift.
3. **Activate**: Execute context-switching logic. Verify that all environment variables are isolated and that no "context leakage" occurs between active projects.
4. **Audit**: Log every environment activation and path repair to `codex_redundancy.log` for reliable operational tracking.
5. **Safety**: Forensic isolation. No project metadata, directory structures, or path information may leave the local hardware.

# Workflows
- **Environment Isolation Audit**: Before every context switch, verify that the previous environment's variables have been cleared.
- **Manifest Health Check**: Compare active project hashes against the "Last Known Good" (LKG) state for failure-proof stability.
