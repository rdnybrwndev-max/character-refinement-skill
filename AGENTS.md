<!-- BEGIN claude-project:design-studio (generated from agent-hub/claude-projects/design-studio/INSTRUCTIONS.md; edit there, not here) -->
## Claude project rules: Design Studio

> MANDATORY on every design turn: read and follow DESIGN-WORKFLOW.md in github.com/rdnybrwndev-max/design-skills (`~/projects/design-skills/DESIGN-WORKFLOW.md`).

# Design Studio

## Goal
Design and refine visuals with Open Design on the Mac Studio; maintain the design skills library.

## Where the work happens
- Repositories: rdnybrwndev-max/design-skills (most tasks), rdnybrwndev-max/character-refinement-skill.
- Branch from the default branch. Name branches <area>/<short-task>. Open a PR when the task is done and tests pass; do not merge.
- Computers: tests, builds and simulator runs go to the Mac mini sandbox first, as agent-hub AGENTS.md "Where work runs" says. Signing, TestFlight uploads and release builds run on the Mac mini too, with Xcode Cloud, then GitHub Actions, as backup. Use Codex Cloud when the mini can't do the job, and GitHub Actions for pull request checks. Keep the Mac Studio for Rodney's live work, Open Design and local-only tools. Never use the Grok Bot box.

## How a thread works
1. Read CLAUDE.md and HANDOFF.md in every repo you touch before changing anything.
2. Run the repo's test or build command before opening a PR. Say in the PR body what you ran.
3. If you can't reach something you need (a repo, secret, API, connector), say exactly what's missing in your first message and stop. Don't mock or guess.
4. Ask before: deleting data, changing deploy config or production servers, sending anything to clients.
5. Before finishing, update HANDOFF.md (rewrite Current state, append to Session log), commit, and push.

## Conventions
- Keep CLAUDE.md short and repo-specific; cross-repo rules live here.
- Save any correction the user asks to be remembered in project memory.

## Reporting
Short. What changed, the PR link, what's next, decisions you need from Rodney.

## Keep this project current
Every run ends by updating agent-hub/claude-projects/design-studio/HANDOFF.md and the repo HANDOFF.md.
<!-- END claude-project:design-studio -->
