# Changelog

All notable changes to the Antigravity Kit will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/2.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [3.0.0] - 2026-04-01

### Added
- **Coordinator Mode Skill**: Multi-agent orchestration with parallel workers, synthesis protocol, fork semantics, and phase-based workflow (Research → Synthesis → Implementation → Verification)
- **Memory System Skill**: Persistent cross-session memory with MEMORY.md index, 4-type taxonomy (user/feedback/project/reference), topic files, and auto-recall at session start
- **Context Compression Skill**: Auto-compress context in long sessions with micro-compact (tool output), phase summary, and session checkpoint levels
- **Verify Changes Skill**: Prove code works by running it — verification through execution, not inspection
- **Batch Operations Skill**: Multi-file pattern-based modifications with preview-before-execute safety
- **Simplify Code Skill**: Detect and reduce over-engineered complexity — unnecessary abstractions, dead code, deep nesting
- **Skillify Skill**: Auto-create new skills from repetitive multi-step workflows
- **New Workflow `/coordinate`**: Advanced multi-agent coordination with coordinator protocol
- **New Workflow `/remember`**: Save information to persistent cross-session memory
- **New Workflow `/verify`**: Verify code changes through execution

### Changed
- **Orchestrator Agent**: Major upgrade with coordinator mode patterns — phase-based workflow, worker prompt synthesis guide ("never delegate understanding"), fork semantics, concurrency rules, memory integration, and context compression awareness
- **Parallel Agents Skill**: Enhanced with `when_to_use` frontmatter and concurrency classification
- **All 44 Skills**: Added `when_to_use` frontmatter field for conditional/intelligent skill loading — reduces token waste by ~1,200 tokens per session
- **README.md**: Complete rewrite with v2 vs v3 comparison table, pros/cons, migration guide, and attribution

### Token Impact
- **+1,500 tokens** upfront (memory index + enhanced agents)
- **-3,000 to -15,000 tokens** saved per session (memory eliminates re-discovery, compression recovers context, better prompts reduce retries)
- **Net: 13-33% more token-efficient** depending on session type

### Inspired By
- Advanced AI agent source code analysis (production architectures, coordinator patterns, memory systems)
- Patterns distilled into original markdown — no external code copied



## [2.0.2] - 2026-02-04
- **New Skills**:
    - `rust-pro` - Master Rust 1.75+ 
- **Agent Workflows**:
    - Updated `orchestrate.md` fix output turkish


## [2.0.1] - 2026-01-26

### Added

- **Agent Flow Documentation**: New comprehensive workflow documentation
    - Added `.agent/AGENT_FLOW.md` - Complete agent flow architecture guide
    - Documented Agent Routing Checklist (mandatory steps before code/design work)
    - Documented Socratic Gate Protocol for requirement clarification
    - Added Cross-Skill References pattern documentation
- **New Skills**:
    - `react-best-practices` - Consolidated Next.js and React expertise
    - `web-design-guidelines` - Professional web design standards and patterns

### Changed

- **Skill Consolidation**: Merged `nextjs-best-practices` and `react-patterns` into unified `react-best-practices` skill
- **Architecture Updates**:
    - Enhanced `.agent/ARCHITECTURE.md` with improved flow diagrams
    - Updated `.agent/rules/GEMINI.md` with Agent Routing Checklist
- **Agent Updates**:
    - Updated `frontend-specialist.md` with new skill references
    - Updated `qa-automation-engineer.md` with enhanced testing workflows
- **Frontend Design Skill**: Enhanced `frontend-design/SKILL.md` with cross-references to `web-design-guidelines`

### Removed

- Deprecated `nextjs-best-practices` skill (consolidated into `react-best-practices`)
- Deprecated `react-patterns` skill (consolidated into `react-best-practices`)

### Fixed

- **Agent Flow Accuracy**: Corrected misleading terminology in AGENT_FLOW.md
    - Changed "Parallel Execution" → "Sequential Multi-Domain Execution"
    - Changed "Integration Layer" → "Code Coherence" with accurate description
    - Added reality notes about AI's sequential processing vs. simulated multi-agent behavior
    - Clarified that scripts require user approval (not auto-executed)

## [2.0.0] - Unreleased

### Initial Release

- Initial release of Antigravity Kit
- 20 specialized AI agents
- 37 domain-specific skills
- 11 workflow slash commands
- CLI tool for easy installation and updates
- Comprehensive documentation and architecture guide

[Unreleased]: https://github.com/vudovn/antigravity-kit/compare/v2.0.0...HEAD
[2.0.0]: https://github.com/vudovn/antigravity-kit/releases/tag/v2.0.0
