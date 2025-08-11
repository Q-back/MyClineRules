# How to commit
Do the work used asked for, but bear in mind you should (eventually) reasonably
split your work to multiple commits.

Don't do many unrelated changes at once, instead use
use `git commit` for each change (or bug or feature) to maintain a
clean history and to easily track what's happening in the project.

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
