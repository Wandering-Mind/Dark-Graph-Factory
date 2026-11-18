# Dark Graph Factory

## An Autonomous Software Factory With Institutional Memory

Dark Graph Factory is a reusable multi\-agent software organization built in BAND Desktop.

The factory is designed to plan, research, implement, verify, and improve software autonomously through collaboration between specialized agent seats. Rather than relying on a single coding agent, Dark Graph Factory distributes responsibility across multiple roles with explicit ownership, documented handoffs, independent review, and persistent organizational memory.

For the BAND Dark Factory Buildathon, Dark Graph Factory autonomously builds **Dossier**, a company\-research service that discovers and verifies company information using WebRouter and Nimble.

---

## Core Idea

Traditional AI coding workflows often operate as isolated sessions.

A task arrives.

Code is generated.

The session ends.

Knowledge disappears.

Dark Graph Factory treats software delivery as an organizational process.

The factory preserves:

- successful implementation patterns
- architectural decisions
- research findings
- review outcomes
- recurring failures
- lessons learned

This accumulated knowledge reduces repeated work and improves future delivery.

---

## Factory Architecture

                         HUMAN

                           │

                           ▼

                    COORDINATOR

                           │

        ┌──────────────────┼──────────────────┐

        │                  │                  │

        ▼                  ▼                  ▼

 RESEARCH ENGINEER   SOFTWARE ENGINEER   VERIFICATION ENGINEER

        │                  │                  │

        └────────────┬─────┴─────┬────────────┘

                     │           │

                     ▼           ▼

                   NIMBLE     VALIDATION

                \+ WEBROUTER   \+ TESTING

                     │

                     ▼

              KNOWLEDGE CURATOR

                     │

                     ▼

                   COGNEE

---

## Agent Seats

### Coordinator

Plans work, decomposes tasks, manages stage progression, coordinates handoffs, and produces final reports.

### Research Engineer

Acquires external information, gathers evidence, resolves uncertainty, and supports implementation decisions.

### Software Engineer

Implements functionality, maintains architecture, writes tests, and produces committed revisions.

### Verification Engineer

Reviews implementation independently, validates requirements, executes testing, and rejects incomplete or incorrect work.

### Knowledge Curator

Maintains institutional memory, captures lessons learned, records decisions, and preserves reusable knowledge for future tasks.

---

## Factory Workflow

Task

  ↓

Coordinator

  ↓

Research Engineer

  ↓

Software Engineer

  ↓

Verification Engineer

  ↓

Knowledge Curator

  ↓

Future Work

If verification fails:

Verification Engineer

         ↓

Software Engineer

         ↓

Verification Engineer

The factory iterates until requirements are satisfied or a blocker is formally recorded.

---

## Design Principles

### Separation of Responsibilities

Each seat owns a distinct function.

### Independent Verification

No seat approves its own work.

### Explicit Handoffs

Work transitions are documented and traceable.

### Organizational Memory

The factory preserves knowledge rather than repeating work.

### Reusability

Agent mandates are generic and can be applied to many software projects.

### Autonomous Operation

Once a task is dispatched, seats coordinate and resolve implementation decisions internally until completion or an explicit blocker is reported.

---

## Technology Stack

### Collaboration

- BAND Desktop

### Research

- Nimble
- WebRouter

### Knowledge Management

- Cognee

### Implementation

- Python
- FastAPI
- Docker

### Validation

- Automated testing
- Harness validation
- Independent agent review

---

## Repository Guide

README.md

FACTORY.md

mandates/

room.json

dossier\-runway.com.json

stage\-1/

stage\-2/

stage\-3/

stage\-4/

### README.md

Project overview and repository navigation.

### FACTORY.md

Factory architecture, workflow, design rationale, metrics, and lessons learned.

### mandates/

Generic seat mandates used during the submitted run.

### room.json

Full BAND session export.

### stage\-N/

Source code and deliverables produced by the factory.

---

## What We Built

Dark Graph Factory demonstrates that a software organization can be represented as a collection of specialized AI agents working together toward a common goal.

Rather than optimizing a single agent, we focused on:

- reusable workflows
- distributed ownership
- independent review
- research efficiency
- persistent organizational memory

The result is a software factory that not only produces software, but continuously improves how it produces software.

---

## Tagline

**A software factory that remembers what it learns.**

