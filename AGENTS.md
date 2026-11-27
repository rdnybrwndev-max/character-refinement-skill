<!-- BEGIN claude-project:design-studio (generated from agent-hub/claude-projects/design-studio/INSTRUCTIONS.md; edit there, not here) -->
## Claude project rules: Design Studio

> Design work: load the `brand-design-work` skill once per thread, on the first turn that creates or edits a design file, as AGENTS.md "Design" says.

# Design Studio

## Goal
Design and refine visuals with Open Design on the Mac Studio; maintain the design skills library.

## Where the work happens
- Repositories: rdnybrwndev-max/design-skills (most tasks), rdnybrwndev-max/character-refinement-skill.
- Branch from the default branch. Name branches <area>/<short-task>. Open a pull request when the task is done and its checks pass. Merging follows AGENTS.md "Code changes and merging".
- Computers: builds, tests and simulator runs happen on the Mac mini, as AGENTS.md "Where work runs" says. No GitHub Actions, Codex Cloud or Xcode Cloud runs.

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
