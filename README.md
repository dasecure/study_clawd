# 📚 Study Clawd

System prompts and workspace files for building AI agents like [Clawdbot](https://github.com/clawdbot/clawdbot).

## Files

| File | Purpose |
|------|---------|
| `AGENTS.md` | Agent behavior, memory management, workspace rules |
| `SOUL.md` | Personality, tone, core values |
| `USER.md` | Info about the human you're helping |

## Skills

Specialized knowledge modules loaded into the agent's context:

| Skill | Expertise |
|-------|-----------|
| `skills/coding.md` | Full-stack development, best practices, code review |
| `skills/electrical-engineering.md` | Circuits, embedded systems, PCB design, IoT |
| `skills/marketing.md` | Growth, content, paid acquisition, analytics |
| `skills/seo.md` | Technical SEO, on-page, off-page, local SEO |

## How It Works

These files are loaded into the AI's context at the start of each session:

```
┌─────────────────────────────────────────┐
│           SYSTEM PROMPT                 │
│  ┌─────────────────────────────────┐    │
│  │  AGENTS.md (how to behave)      │    │
│  │  SOUL.md (who you are)          │    │
│  │  USER.md (who you're helping)   │    │
│  │  memory/*.md (recent context)   │    │
│  └─────────────────────────────────┘    │
└─────────────────────────────────────────┘
              ↓
        AI has persistent
        "memory" and personality
```

## Usage

1. Fork this repo
2. Edit the files to match your preferences
3. Point your AI agent to load these files into its system prompt

## See Also

- [Clawdbot](https://github.com/clawdbot/clawdbot) — The full AI agent framework
- [MiniBot](/home/clawd/clawd/minibot) — A minimal ~200 line implementation

## License

MIT
