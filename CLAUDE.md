# CLAUDE.md — character-refinement-skill

## What this repo is
A single agent skill (`skill.md`, skill name `character-refinement-3d`) that audits and refines 2D character concept sheets into consistent, Blender-ready turnarounds for a painterly, Monet-inspired side-scrolling 3D platformer.

## Structure
- `skill.md` — the skill itself: YAML frontmatter (`name`, `description`) + workflow (Audit → Lock design → Painterly style → Platformer readability → Deliverables) and Rules.
- `README.md` — one-line project description.
- `CLAUDE.md`, `HANDOFF.md` — agent working notes.

## Conventions
- Keep frontmatter valid: `name` kebab-case, `description` states when to use the skill.
- Workflow steps stay numbered and ordered; the audit output format is a table `issue | where (view) | severity | fix`.
- Write decisively ("decide, don't hedge"); prefer short bullet lists.
- Never invent a new character; the skill refines the provided one.
- One change per commit with a clear message; keep a change log in HANDOFF.md.

## Commands
No build or tests. Typical: `git pull`, edit `skill.md`, `git commit`, `git push origin main`.
To use in Claude Code, copy/symlink into a skills dir, e.g. `~/.claude/skills/character-refinement-3d/SKILL.md`.

<!-- claude-project:start (managed by claude-config/bin/sync-project-context.sh) -->
## Claude project
- **Design Studio** (claude.ai/code): Design and refine visuals with Open Design on the Mac mini; maintain the design skills library.
  Full instructions: OPOSEO/claude-config claude-projects/design-studio/INSTRUCTIONS.md
- Every run ends by updating this repo's HANDOFF.md and the project HANDOFF.md above (CLAUDE.md too if rules changed).
<!-- claude-project:end -->
