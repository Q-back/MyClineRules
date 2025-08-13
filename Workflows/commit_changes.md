# commit_changes.md
Summarize all the changes from this task and perform commit.

## Commit message
Each commit created by you should start with `AI: ` followed by short commit title
starting with capital letter and without dot (`.`) at the end.
The commit title should be written in imperative.
Then you should add empty line and task description.
Try to not exceed 80 or 100 characters per line in commit message.

### Example:
"""
AI: Refactor timer to be datetime-based not interval-based

Previously timer component utilized `setInterval` to increment
the amount of seconds already spent on task every 1 second.
It was prone to errors when user e.g. reloaded tab.
`datetime-based` approach has no such issues.
"""

## Use MCP for git
Prefer to interact with `git` using MCP servers (Git tools).
When you commit changes using terminal - remember to check terminal output to make sure
that no git hook failed
