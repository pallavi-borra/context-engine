# Context System - FlowSpace Example

A composable system of context artifacts for AI-assisted operations.

## Purpose

This folder contains structured business context for **FlowSpace** - a project management and collaboration platform designed specifically for remote creative teams. This serves as a realistic example of how to populate the context template with actual business information.

## About FlowSpace

FlowSpace helps remote creative teams (design agencies, marketing teams, content studios) manage projects, collaborate visually, and deliver work on time without the chaos of context-switching between tools.

**Tagline:** Where creative teams actually get work done.

## Folder Structure

```
context/
├── identity/       # Who we are (mission, values, voice)
├── offerings/      # What we sell (products, pricing)
├── customers/      # Who we serve (personas, journey)
├── market/         # Where we compete (landscape, competitors)
├── operations/     # How we work (team, processes)
├── strategy/       # Where we're going (goals, initiatives)
└── .archive/       # Deprecated documents
```

## How to Use

### Loading Context

Before any task, load the relevant context files:

```
Load these context files:
- context/identity/company-brief.md
- context/customers/customer-personas.md

Then [your task].
```

### Common Combinations

| Task | Load These |
|------|------------|
| Marketing copy | identity + customers + offerings |
| Product decisions | customers + offerings + strategy |
| Competitive response | market + offerings + identity |
| Sales messaging | customers + offerings |
| Strategic planning | strategy + market + operations |

## Document Structure

Every context document includes:

1. **YAML front matter** - Machine-readable metadata
2. **Metadata table** - Human-readable summary
3. **Change history** - Version tracking
4. **Purpose & when to load** - Usage guidance
5. **Content sections** - The actual context
6. **Open questions** - Unresolved items
7. **See also** - Cross-references

## Note

This is an example implementation. Use the `context-template` folder as your starting point and replace FlowSpace-specific content with your own business information.

