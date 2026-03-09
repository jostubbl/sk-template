# sk-template

A [Spec Kit](https://github.com/github/spec-kit) enabled repository template for scaffolding new projects with Spec-Driven Development (SDD) workflows.

## What is Spec Kit?

Spec Kit is a toolkit that helps teams practice Spec-Driven Development — a methodology where clear specifications guide implementation, especially when working with AI coding assistants like GitHub Copilot.

## What's Included

This template provides the full Spec Kit setup for GitHub Copilot (v0.2.0):

- **`.github/agents/`** — GitHub Copilot agent command files for the full SDD workflow
- **`.github/prompts/`** — Prompt shortcuts for triggering Spec Kit commands in Copilot Chat
- **`.specify/templates/`** — Document templates (spec, plan, tasks, constitution, checklist)
- **`.specify/scripts/bash/`** — Helper scripts for managing features and branches
- **`.specify/memory/constitution.md`** — Project constitution (customize with your principles)
- **`specs/`** — Directory where feature specifications are stored

## Getting Started

### 1. Customize the Constitution

Edit `.specify/memory/constitution.md` to define your project's core principles, constraints, and governance rules. You can also use the `/speckit.constitution` command in GitHub Copilot Chat to generate it interactively.

### 2. Create a Feature Specification

In GitHub Copilot Chat, use:

```
@workspace /speckit.specify Add user authentication with email and password
```

This will create a feature branch and populate a specification in `specs/`.

### 3. Generate an Implementation Plan

```
@workspace /speckit.plan
```

### 4. Break Into Tasks

```
@workspace /speckit.tasks
```

### 5. Implement

```
@workspace /speckit.implement
```

## Available Commands

| Command | Description |
|---------|-------------|
| `/speckit.specify` | Create a feature specification |
| `/speckit.clarify` | Clarify specification requirements |
| `/speckit.plan` | Generate an implementation plan |
| `/speckit.tasks` | Break the plan into actionable tasks |
| `/speckit.implement` | Execute the implementation plan |
| `/speckit.checklist` | Generate a checklist for a domain |
| `/speckit.analyze` | Analyze the project for consistency |
| `/speckit.constitution` | Create or update the project constitution |
| `/speckit.taskstoissues` | Convert tasks to GitHub Issues |

## Learn More

- [Spec Kit on GitHub](https://github.com/github/spec-kit)
- [Spec-Driven Development Guide](https://github.com/github/spec-kit/blob/main/spec-driven.md)
