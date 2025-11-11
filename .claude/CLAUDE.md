# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

---

# A2I Curriculum Repository Guidelines

## Repository Overview

**Type:** Educational curriculum repository (documentation-focused, not software)

**Purpose:** Open-source Master of Science in Applied Artificial Intelligence & Business Systems (A²I) curriculum at UIUC Gies College. Trains "system orchestrators" who align people, data, and AI agents toward business and societal value.

**Core Philosophy:** "Capability is cheap; coherence is scarce" - focuses on leadership, governance, and reflexive learning rather than pure technical training.

**Program Structure:** 36 credits, twelve 8-week courses, designed for working professionals via Coursera (content) + Canvas (assessments) + Google Cloud (labs) + GitHub (open development).

## Architecture & Directory Structure

### Key Directories

- **`docs/curriculum/`** - Academic content: core courses (A²I 601-606), electives, labs/studios (621-623), capstone (699), learning outcomes
- **`docs/pedagogy/`** - Four-model framework: Reflexive Learning, Cyber-Social Learning, AI Feedback & Assessment, Empowerment ↔ Plasticity
- **`docs/platform/`** - Technical delivery: Canvas integration, Coursera, GCP stack, GitHub workflows
- **`docs/governance/`** - Policies: academic integrity, AI use charter, data privacy
- **`docs/entrepreneurship/`** - Venture creation track and iVenture Accelerator integration
- **`docs/context/conversation.md`** - Founding conversation transcript; update with major decision rationale
- **`.github/workflows/`** - Active automation (AI review, auto-labeling, Canvas sync)
- **`automation/`** - Development area for workflows and issue templates

### 8-Week Course Template Standard

All courses follow this structure:
- Week 0: Orientation + AI-use charter
- Weeks 1-8: Mixed delivery (Coursera videos, Canvas assignments, GCP labs)
- Week 8: Oral viva + reflection
- Assessment: 50% projects, 20% auto-checks, 20% viva, 10% peer critique

### Citation Convention

Use `【F:path†L#】` format when referencing source documents to maintain traceability.

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

## Automation & Workflows

### Active GitHub Actions

**AI-Assisted Review** (`.github/workflows/ai_review.yml`)
- Triggers on PRs affecting `docs/**/*.md`
- Performs markdown linting, link checking, automated review comments
- Skeleton implementation - AI integration pending

**Auto-label Issues** (`.github/workflows/auto_label_issues.yml`)
- Triggers on issue creation/edit
- Auto-applies labels: curriculum, platform, governance, pedagogy, entrepreneurship, priority
- Uses template type and content keywords

**Canvas Sync** (`.github/workflows/sync_to_canvas.yml`)
- Triggers on push to main affecting `docs/curriculum/**` or manual dispatch
- Syncs curriculum to Canvas LMS via API
- Requires CANVAS_API_URL and CANVAS_API_TOKEN secrets
- Placeholder implementation

### Disabled Workflows
- ~~`curriculum_change_log.yml`~~ - Changelog automation (removed per policy above)

## Contribution Process

**For Curriculum Changes:**
1. Use `.github/ISSUE_TEMPLATE/curriculum_update.yml` template
2. Provide clear rationale and learning outcomes impact
3. Reference relevant pedagogy
4. Submit PR with changes

**Issue Templates:**
- `curriculum_update.yml` - Primary template for content changes
- `bug_report.yml` - Documentation errors
- `feedback.yml` - General feedback

## Program Metrics & Continuous Improvement

The program prioritizes coherence, inclusion, entrepreneurship, governance, and open development as core success themes. Detailed metrics and assessment frameworks are documented in:

- **`docs/metrics.md`** - Program success metrics aligned with "Capability is cheap; coherence is scarce" philosophy
- **`docs/pedagogy/business_coherence_scorecard.md`** - Student-level assessment tool for measuring coherence
- **`docs/research/2025-11-first-principles-review.md`** - Annual curriculum review methodology

**Philosophy:** Continuous improvement over fixed roadmaps. Success is measured by coherence (alignment across strategy-operations-governance), not by time-bound deliverables.
