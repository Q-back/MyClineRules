# Write plan

## Legend
`plan` is `.md` file in `work_notes/`.
Each `plan` must include `Plan structure` described below.

## Plan structure
Each plan should describe:
- Problem
- Definition of done
- Solution
- Most important issue

## When you need to work in phases
Sometimes problems are big.
In this scenario good approach is to create one "abstract" `plan` file and follow
up with dedicated `plan` files for each phase.

## Communication
Outlining, rich markdown and emojis help to structure the `plan`. 

## No code changes
Do not touch code.
Don't make any other changes than `plans`.
Ideally you shouldn't touch anything outside `work_notes/` directory.

## Plan files location
All plans should be placed in `work_notes/` directory.
Create this directory if it doesn't exist yet.

## Auto commit
Write the `plan` user asked for.

Don't do many unrelated changes at once, instead use
use `git commit` for each reasonable plan stage to maintain a
clean history and to easily track what's happening in the project.

### Commit message
Each commit created by you should start with `AI: ` followed by short commit title
starting with capital letter and without dot (`.`) at the end.
The commit title should be written in imperative.
Then you should add empty line and task description.
Try to not exceed 80 or 100 characters per line in commit message.

#### Example:
"""
AI: Refactor timer to be datetime-based not interval-based

Previously timer component utilized `setInterval` to increment
the amount of seconds already spent on task every 1 second.
It was prone to errors when user e.g. reloaded tab.
`datetime-based` approach has no such issues.
"""

### Use MCP for git
Prefer to interact with `git` using MCP servers.
When you commit changes using terminal - remember to check terminal output to make sure
that no git hook failed

## Ensure you understand
When you work on a task ensure you understand exactly what you're expected to do.
Make sure you know what's the expected output and confirm you understand it properly.
Don't hesitate to ask if something's not clear. 
