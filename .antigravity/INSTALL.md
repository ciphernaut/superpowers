# Installing Superpowers for Antigravity

Follow these steps to enable Superpowers skills in your Antigravity environment.

## 1. Clone the repository

```bash
git clone https://github.com/obra/superpowers.git ~/.agents/superpowers
```

## 2. Register skills

Create a symlink so Antigravity discovers the skills:

```bash
mkdir -p ~/.agents/skills
ln -s ~/.agents/superpowers/skills ~/.agents/skills/superpowers
```

## 3. Verify

Start a new session and mention "superpowers". The agent should acknowledge the discovery of Superpowers skills.
