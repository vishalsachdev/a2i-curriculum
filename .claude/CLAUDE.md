# A2I Curriculum Repository Guidelines

## Changelog Management

**Automation Status:** Disabled (manual updates only)

**When to Update CHANGELOG.md:**
Update the changelog only for significant milestones:
- New version releases (v0.2, v0.3, etc.)
- Major structural changes (course additions/removals, restructuring)
- Significant feature additions (new documentation sections, major tools)

**When NOT to Update:**
- Minor typo fixes
- Small documentation tweaks
- Formatting changes
- Incremental content additions

**Philosophy:**
Keep the changelog high-level and curated, not granular. It should tell the story of major evolution, not track every edit.

## Workflow Standards

**Branch Structure:**
- Main branch: `main`
- Feature branches: Use descriptive names (avoid AI-generated long branch names)
- Clean up merged branches promptly

**Commit Messages:**
- Focus on "why" over "what"
- Reference related issues/PRs when applicable
- Use conventional commit format for clarity

## Documentation Standards

**Core Principles:**
- Maintain coherence across docs/curriculum/, docs/pedagogy/, docs/platform/
- Cross-reference related documents using relative links
- Keep context/conversation.md updated with major decision rationale
- Use citation format 【F:path†L#】 when referencing source documents

## Automation

**Active Workflows:**
- `.github/workflows/ai_review.yml` - AI-based PR review
- `.github/workflows/auto_label_issues.yml` - Issue labeling
- `.github/workflows/sync_to_canvas.yml` - Canvas LMS sync

**Disabled Workflows:**
- ~~`curriculum_change_log.yml`~~ - Changelog automation (removed)
