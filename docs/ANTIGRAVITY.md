# Antigravity Superpowers Guide

This document contains verbose documentation, historical context, and templates for the Antigravity integration of the Superpowers framework. It is intended as a deep-dive resource when the minimal protocol requires elaboration.

## Historical Context
The Antigravity adaptation was created to ground the agent in high-discipline workflows while maintaining awareness of its native toolset.

## Detailed Tool Mapping
Although Antigravity agents automatically use native tools, this table serves as a reference for cross-platform compatibility.

| Superpowers Term | Antigravity Tool | Use Case |
|------------------|------------------|----------|
| `Skill`          | `view_file`      | Grounding in specific instructions |
| `TodoWrite`      | `task_boundary`  | UI updates and persistence |
| `Bash`           | `run_command`    | Terminal execution |
| `Notify`         | `notify_user`    | Communication |

## Standard Templates

### task.md Template
```markdown
# Task: [Objective]

- [/] [Task 1] <!-- id: 0 -->
    - [ ] [Sub-task] <!-- id: 1 -->
- [ ] [Task 2] <!-- id: 2 -->
```

### walkthrough.md Template
```markdown
# Walkthrough - [Objective]

## Changes Made
- Summary of changes

## Verification
### Automated Tests
- Command + Results

### Manual Verification
- Evidence of work
```

## Installation Reference
### Manual Symlinking
```bash
mkdir -p .agents/workflows
ln -s "$(pwd)/.agents/workflows/superpowers.md" .agents/workflows/superpowers.md
```
