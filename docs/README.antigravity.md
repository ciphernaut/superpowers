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
git clone https://github.com/obra/superpowers.git ~/skills/superpowers
```

### 2. Register Skills

Choose the scope that fits your needs:

#### Global (All Projects)
```bash
mkdir -p ~/.gemini/antigravity/skills
ln -s ~/skills/superpowers/skills ~/.gemini/antigravity/skills/superpowers
```

#### Workspace-specific (This Project Only)
```bash
mkdir -p .agent/skills
ln -s ~/skills/superpowers/skills .agent/skills/superpowers
```

## How It Works

Antigravity uses native skill discovery. By symlinking the `skills/` directory into a recognized skills folder, the agent automatically finds and indexes available skills.

### Discovery Mechanism
The agent reads the `name` and `description` from the YAML frontmatter of `SKILL.md` in each skill folder at the start of a session. It uses this information to determine which skills are relevant to your task.

### Activation
The full content of a skill is only loaded ("activated") when the agent determines it is necessary for the current operation.

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
- **Skills not found**: Verify the symlink points to the correct `skills/` directory:
    - Global: `~/.gemini/antigravity/skills/superpowers`
    - Workspace: `.agent/skills/superpowers`
- **Context missing**: Ensure you have invoked the `using-superpowers` skill at the start of your session.
