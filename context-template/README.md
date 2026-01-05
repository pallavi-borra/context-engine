# Context System Template

A composable system of context artifacts for AI-assisted operations.

## Purpose

This folder contains structured business context templates that AI agents can load to perform tasks with precision. Instead of re-explaining your business every conversation, agents load the relevant context files and operate with full knowledge.

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

### Getting Started

1. **Copy this template folder** to your project as `context/`
2. **Fill in each document** with your actual business information
3. **Remove template placeholders** like `[Your Name]`, `[DATE]`, etc.
4. **Update cross-references** to match your actual file structure
5. **Mark documents as Active** once populated (change Status from "Template" to "Active")

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

## Implementation Phases

### Phase 1: Foundation (Start Here)
- [ ] Complete `identity/company-brief.md`
- [ ] Complete `customers/customer-personas.md`
- [ ] Complete `offerings/offerings-overview.md`

### Phase 2: Core Context
- [ ] Complete `market/market-overview.md`
- [ ] Complete `strategy/goals.md` (or strategy-overview.md)
- [ ] Add any additional identity documents (messaging, voice, etc.)

### Phase 3: Depth
- [ ] Add specialized documents as needed
- [ ] Establish cross-references between documents
- [ ] Test with actual AI agent tasks

### Phase 4: Maintenance (Ongoing)
- [ ] Review quarterly for staleness
- [ ] Update after major business changes
- [ ] Archive deprecated documents

## Document Naming Convention

- Use descriptive lowercase names with hyphens: `customer-personas.md`, `market-overview.md`
- Template documents can use `.template.md` suffix (optional)
- Keep names simple and clear

## Status Values

- **Template** - Empty template, ready to fill
- **Draft** - Initial creation, not yet validated
- **Active** - Current, validated, ready for use
- **Under Review** - Being updated or validated
- **Deprecated** - No longer current

## Maintenance

Use the Context Sculpting skill to:
- Update documents after conversations
- Run audits to catch inconsistencies
- Interview to fill in gaps

See: `../skills/context-sculpting/SKILL.md` for detailed workflows.
