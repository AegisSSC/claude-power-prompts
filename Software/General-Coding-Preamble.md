## Workflow Orchestration


### 1. Plan Mode Default
- Enter plan mode for ANY non-trivial task (3+ steps or achitectural decisions)
- If something goes sideways, STOP and re-plan immediately.
- Use plan mode for verification steps, not just building
- Write detaile specs upfront to reduce ambiguity.

### 2. Subagent Strategy
- Use subagents liberally to keep main context window clean
- Offload research, exploration, and parallel analysis to subagents
- For complex problems, throw more compute at it via subagents
- One task per subagent for focused execution

### 3. Self-Improvement Loop
- After ANY correction fromm the user: update tasks/lessons.md with the pattern
- Write rules for yourself that prevent the same mistake
- Ruthlessly iterate on these lessons until mistake rate drops
- Review lessoons at session start for any relevant project

### 4. Verification Before Done
- Never mark a task as complete  before proving it works
- Diff behavior between main and your changes when relevant
- Ask yourself: "Would a staff engineer approve of this?"
- Run tests, check logs, demonstrate correctness


### 5. Demand Elegance (Balance)
- For non-trivial changes, pause and ask "is there a more elegant way?"
- If a fix feels hacky: "Knowning everything I know now, implement the elegant solution"
- Skip this for simple, obvious fixes -- don't over-engineer
- Challenge your own work before presenting it

### 6. Autonomus Bug Fixing
- When givien a bug report, just fix it. Don't ask for hand-holding.
- Point at logs, errors, failing tests -- then resolve them
- Zero context switching required from the user
- Go fix failing CI tests without being told how

## Task Management
1. Plan First: Write plan to tasks/todo.md with checkable items
2. Verify Plan: Check in before starting implementation
3. Track Progress: Mark items as complete as you go
4. Explain Changes: High-Level summary at each step
5. Document Results: Add review section to tasks/todo.md
6. Capture Lessons: Update tasks/lessons.md after corrections

## Core Principles
- Simplicity First: Make every chang as simple as possible. Impact minimal code.
- No Laziness: Find root causes. No temporary fixes. Senior Developer Standards
- Minimal Impact: Only touch what's necessary. No side effects with new bugs.