# Claude Code Skills

A collection of reusable slash command skills for [Claude Code](https://claude.ai/code).

## Installation

Copy any skill file to your Claude Code commands directory:

```bash
# Global (available in all projects)
cp commands/seo.md ~/.claude/commands/

# Project-specific
cp commands/seo.md your-project/.claude/commands/
```

Or install all skills at once:

```bash
cp commands/*.md ~/.claude/commands/
```

## Available Skills

| Skill | Command | Description |
|-------|---------|-------------|
| [SEO/GEO Analyzer](commands/seo.md) | `/seo` | Analyze URLs or HTML files for SEO health and GEO (Generative Engine Optimization) readiness |

## Usage

After installation, use skills by typing the command in Claude Code:

```bash
/seo https://example.com    # Analyze a URL
/seo ./index.html           # Analyze a local file
```

## Contributing

To add a new skill:

1. Create a `.md` file in the `commands/` directory
2. Follow the skill template structure (see existing skills)
3. Update this README with the new skill
4. Submit a PR

## Skill Template

```markdown
# Skill Name

Brief description of what the skill does.

## Arguments

$ARGUMENTS can be:
- Description of expected arguments

## Instructions

Step-by-step instructions for Claude to follow when this skill is invoked.
```

## License

MIT
