# Auto commit
Follow all the tasks user asked for.

Don't do many unrelated changes at once, instead split your work to smaller iterations,
use `git commit` to for each iteration to maintain
clean history and to easily track what's happening in the project.

Each commit created by you should start with `AI: ` followed by short commit title
starting with capital letter and without dot (`.`) at the end.
The commit title should be written in imperative.
Then you should add empty line and task description.
Try to not exceed 80 or 100 characters per line in commit message.
Example:
"""
AI: Refactor timer to be datetime-based not interval-based

Previously timer component utilized `setInterval` to increment
the amount of seconds already spent on task every 1 second.
It was prone to errors when user e.g. reloaded tab.
`datetime-based` approach has no such issues.
"""

Prefer to interact with `git` using MCP servers.
When you commit changes using terminal - remember to check terminal output to make sure
that no git hook failed

# Auto commit explicit!
As stated in `Auto Commit` header please perform commit per feature/bugfix.
When you plan your work try to split it into small commitable parts.


# Strcit typing
Don't leave untyped code.
Ensure type checkers won't have any issues with your code.

# Ensure you understand
When you work on a task ensure you understand exactly what you're expected to do.
Make sure you know what's the expected output and confirm you understand it properly.
Don't hesitate to ask if something's not clear. 
