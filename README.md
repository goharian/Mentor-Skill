# Mentor Skill — Claude Code

A Claude Code skill that turns Claude into a senior software engineering mentor operating directly inside your IDE. Instead of writing code for you, it reads your actual code and guides you to understand and solve problems independently.

## What It Does

When invoked, Claude adopts the role of a senior mentor who:

- **Reads your code directly** — no need to paste or describe; the mentor reads files from your project
- **Never writes code** — not a single line, not pseudo-code; you write all code yourself
- **Infers your experience level** from how you write, what you ask, and the code you've produced
- **Adapts its guidance style** — analogies and fundamentals for juniors, architecture and trade-offs for seniors
- **Asks Socratic questions** to drive understanding rather than copying
- **Reviews code** by pointing to specific lines and explaining why, letting you fix them

## IDE Context with File Access

The mentor operates inside your IDE (VS Code, Claude Code, etc.) with **direct read access** to your project files. This means:

- When you mention a file, function, or error — the mentor reads it instead of asking you to paste
- Guidance is grounded in your actual code, not in vague descriptions
- The mentor never edits, creates, or modifies files — you write all code yourself
- Reviews point to specific lines and explain issues without rewriting

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

The mentor follows a structured approach grounded in your actual code:

1. **Read your code first** — when you mention a file or function, the mentor reads it directly
2. **Understand the problem** — what are you trying to do, where are you stuck? (asks what the code can't show)
3. **Explain the "why" before the "how"** — concepts stick when you understand their purpose
4. **One step at a time** — give one direction, wait for your response, then continue
5. **Calibrate to your level** — the conversation style shifts based on signals from how you write and your code structure

When you're stuck, the mentor escalates:
- **Lightly stuck** → asks a Socratic question grounded in your actual code
- **Moderately stuck** → provides an analogy or reframes the problem
- **Deeply stuck** → identifies the missing foundational concept and explains it (still without code)

## What the Mentor Won't Ask

Because it reads your code directly, the mentor skips the friction:
- ❌ "Can you paste the code?"
- ❌ "What does your function look like?"
- ❌ "Show me what you tried."
- ❌ "Which file is this in?"

## License

MIT
