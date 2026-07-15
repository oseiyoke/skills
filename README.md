# skills

A collection of [Claude](https://claude.com/claude-code) skills. A skill is a folder with a `SKILL.md` that teaches Claude a repeatable way of working; Claude loads it automatically when a task matches its description.

Free for anyone to use, copy, change, and share, for any purpose. No permission needed, no credit required. See [LICENSE](LICENSE).

## Skills

| Skill | What it does |
|-------|--------------|
| [explain-like-im-a-child](explain-like-im-a-child) | Explains complex technical material the way you would to a smart child: one everyday analogy, simple words, and every finding kept intact. Triggers on "explain like I'm five", "too complex", "simplify", "break it down", or plain confusion. |

## Install a skill

Skills live in `~/.claude/skills/`. Clone this repo, then symlink the skill you want so it stays in sync as the repo updates:

```bash
git clone https://github.com/oseiyoke/skills.git
ln -s "$PWD/skills/explain-like-im-a-child" ~/.claude/skills/explain-like-im-a-child
```

Prefer a fixed copy over a live link? Copy instead of symlink:

```bash
cp -R skills/explain-like-im-a-child ~/.claude/skills/
```

Starting from a clean setup with no skills yet? You can clone the whole repo straight into place:

```bash
git clone https://github.com/oseiyoke/skills.git ~/.claude/skills
```

Either way, the skill is available in your next Claude session. Invoke it explicitly with `/explain-like-im-a-child`, or just let Claude reach for it when your request matches.

## Add a new skill

1. Create `<skill-name>/SKILL.md` with YAML frontmatter (`name`, `description`) followed by the instructions.
2. The `description` is what makes Claude trigger the skill, so say both what it does and when to use it.
3. Add a row to the table above, commit, and push.
