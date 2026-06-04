# TRUST.md

> A proposed open standard for Human–AI Intent Verification, Transparency, and Trust.

## The Problem

AI is becoming increasingly capable.

Modern AI systems can write code, manage infrastructure, analyze documents, make recommendations, automate workflows, and perform complex tasks.

However, intelligence alone does not create trust.

Many AI failures occur not because the AI lacks capability, but because it:

* Misunderstood the user's intent
* Made hidden assumptions
* Chose one interpretation among many
* Failed to explain consequences
* Executed actions the user did not expect

Consider the following request:

> Delete old files from my computer.

What does "old" mean?

* Created over 30 days ago?
* Modified over 30 days ago?
* Not accessed recently?

An AI may perform the correct action for the wrong interpretation.

From the user's perspective, this is still a failure.

---

## The Missing Layer

Today we have:

| Standard        | Purpose                            |
| --------------- | ---------------------------------- |
| README.md       | Explains a project                 |
| CONTRIBUTING.md | Explains how to contribute         |
| AGENTS.md       | Provides instructions to AI agents |
| CLAUDE.md       | Provides Claude-specific guidance  |
| COPILOT.md      | Provides Copilot-specific guidance |

But there is no standard that answers:

> How should an AI verify that it correctly understood the human before acting?

TRUST.md proposes that missing layer.

---

## What is TRUST.md?

TRUST.md is a proposed standard that defines how AI systems should:

* Verify user intent
* Detect ambiguity
* Expose assumptions
* Report confidence
* Explain consequences
* Assess risk
* Request confirmation for critical actions

The goal is simple:

> Increase trust between humans and AI systems.

---

## Trust Protocol

Before executing meaningful actions, AI should follow:

```text
User Request
      ↓
Intent Understanding
      ↓
Ambiguity Detection
      ↓
Assumption Disclosure
      ↓
Confidence Assessment
      ↓
Consequence Preview
      ↓
Risk Classification
      ↓
Confirmation Gate
      ↓
Execution
```

---

## Example

### User Request

> Delete all old files from my Downloads folder.

### Traditional AI

```text
Deleting files older than 30 days...
```

### TRUST.md-Compliant AI

```text
Intent:
Delete old files from Downloads

Possible Ambiguity:
"Old" could mean:
- Creation date
- Modified date
- Last access date

Assumptions:
- You mean modified date
- You want permanent deletion

Risk:
High

Consequence:
Files may be permanently lost

Confirmation Required:
Yes
```

The second approach is slower.

But it is significantly more trustworthy.

---

## Core Principles

### 1. Intent Before Execution

Understanding the request is more important than executing quickly.

### 2. Assumptions Must Be Visible

Hidden assumptions create hidden failures.

### 3. Uncertainty Must Be Exposed

AI should reveal uncertainty rather than pretending confidence.

### 4. Consequences Matter

Users should understand likely outcomes before execution.

### 5. Critical Actions Require Confirmation

High-impact decisions should never be executed blindly.

---

## Vision

The future of AI is not only about making models smarter.

It is also about making them:

* More transparent
* More predictable
* More controllable
* More aligned with human intent

README.md explains projects.

AGENTS.md guides AI.

TRUST.md helps ensure humans and AI understand each other.

---

## Contributing

This repository is an open proposal.

Feedback, discussion, criticism, improvements, examples, and implementations are welcome.

The objective is to explore whether a universal trust protocol can improve Human–AI collaboration.

---

## License

Open for community discussion, experimentation, and implementation.
