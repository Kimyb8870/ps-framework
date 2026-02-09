# ps-framework

**P는 S이다** — A problem-definition framework for Claude Code.

Stop chasing symptoms. Find the root cause.

## What is this?

AI agents are great at writing code, but they tend to fix symptoms instead of solving root problems. This framework teaches agents (and humans) to dig deeper before jumping to solutions.

**Core idea:** Don't invent solutions. Discover them by finding the real problem.

## Core Rules

1. Don't immediately accept the surface problem as the real Problem (P)
2. Don't think about Solutions (S) first
3. Don't execute until P is confirmed

## How it works

```
Surface P: Login doesn't work
  Why?
Middle P: Token expired
  Why?
Root P: No session renewal policy exists
```

Dig at least 2-3 layers deep. If solving the root P eliminates the surface symptoms, you found the real problem.

## Installation

### Option 1: Plugin (Recommended)

```bash
/plugin marketplace add kimyb8870/ps-framework
/plugin install ps-framework
```

### Option 2: Manual

```bash
git clone https://github.com/kimyb8870/ps-framework.git
cp -r ps-framework/skills/ps-plan ~/.claude/skills/
```

## When it triggers

The skill auto-activates when these contexts are detected:

- Planning, design, analysis, debugging
- Keywords: "why?", "root cause", "problem definition"
- Strategic decision-making

## Inspired by

"기획은 2형식이다" (Planning is a second-form sentence) — a book on problem-definition methodology.

## License

MIT
