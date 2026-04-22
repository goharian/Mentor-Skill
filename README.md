# Mentor Skill — Claude Code

A Claude Code skill that turns Claude into a senior software engineering mentor. Instead of writing code for you, it guides you to understand and solve problems independently.

## What It Does

When invoked, Claude adopts the role of a senior mentor who:

- **Never writes code** — not a single line, not pseudo-code
- **Infers your experience level** from how you write and what you ask
- **Adapts its guidance style** — analogies and fundamentals for juniors, architecture and trade-offs for seniors
- **Asks Socratic questions** to drive understanding rather than copying
- **Reviews code** by pointing out issues and explaining why, letting you fix them

## Installation

Copy the `.claude/skills/Mentor/` directory into your project's `.claude/skills/` folder (or your global `~/.claude/skills/` folder for use across all projects).

## Usage

Trigger the skill by typing `/Mentor` in Claude Code, or describe your problem naturally — the skill activates automatically when you ask for help with code, architecture, debugging, or say things like "I'm stuck" or "I don't know how to start."

```
/Mentor I don't understand how async/await works
/Mentor Can you review this function I wrote?
/Mentor I'm stuck on this bug and I've tried everything
```

## Who It's For

- **Junior developers** — building foundational understanding step by step
- **Mid-level developers** — thinking about structure, patterns, and edge cases
- **Senior developers** — design discussions, trade-offs, and architectural thinking
- **Anyone** — entering unfamiliar territory in a new language, framework, or domain

## How the Mentor Guides

The mentor follows a structured approach:

1. **Understand the problem** — what are you trying to do, what have you tried, where are you stuck?
2. **Explain the "why" before the "how"** — concepts stick when you understand their purpose
3. **One step at a time** — give one direction, wait for your response, then continue
4. **Calibrate to your level** — the conversation style shifts based on signals from how you engage

When you're stuck, the mentor escalates:
- Lightly stuck → Socratic question
- Moderately stuck → analogy or concrete framing
- Deeply stuck → backs up to explain the missing foundational concept

## License

MIT
