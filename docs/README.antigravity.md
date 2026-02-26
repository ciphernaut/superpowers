# Superpowers for Antigravity

Complete guide for using Superpowers with the Antigravity platform.

## Quick Install

Tell Antigravity:

```
Read and follow instructions from https://raw.githubusercontent.com/obra/superpowers/refs/heads/main/.antigravity/INSTALL.md
```

## Manual Installation

### 1. Clone Superpowers

```bash
git clone https://github.com/obra/superpowers.git ~/.agents/superpowers
```

### 2. Create Skills Symlink

```bash
mkdir -p ~/.agents/skills
ln -s ~/.agents/superpowers/skills ~/.agents/skills/superpowers
```

## How It Works

Antigravity uses native skill discovery. By symlinking the `skills/` directory into `~/.agents/skills/`, the agent can automatically find and invoke Superpowers skills.

The `using-superpowers` skill is the entry point that ensures you are grounded in the Superpowers framework from the start of every session.

## Usage

### Discovery
Ask Antigravity to list available skills:
```
list available skills
```

### Loading a Skill
Invoke a specific skill:
```
use skill brainstorming
```

## Troubleshooting
- **Skills not found**: Verify the symlink at `~/.agents/skills/superpowers` points to the correct `skills/` directory.
- **Context missing**: Ensure you have invoked the `using-superpowers` skill at the start of your session.
