# code_and_commit.md
## Prefer to write tests
If possible - prefer TDD approach and include writing tests in your plan.
Prefferably tests should be written and committed before the code.

## Strict typing
Don't leave untyped code.
Ensure type checkers won't have any issues with your code.

## Commit your work
Follow these commit instructions:

### How to commit
Do the work user asked for, but bear in mind you should (eventually) reasonably
split your work to multiple commits.

Don't do many unrelated changes at once, instead use
use `git commit` for each change (or bug or feature) to maintain a
clean history and to easily track what's happening in the project.

**Commit message**
Each commit created by you should start with `AI: ` followed by short commit title
starting with capital letter and without dot (`.`) at the end.
The commit title should be written in imperative.
Then you should add empty line and task description.
Try to not exceed 80 or 100 characters per line in commit message.

**Example:**
```
AI: Refactor timer to be datetime-based not interval-based

Previously timer component utilized `setInterval` to increment
the amount of seconds already spent on task every 1 second.
It was prone to errors when user e.g. reloaded tab.
`datetime-based` approach has no such issues.
```

**Use MCP for git**
Prefer to interact with `git` using MCP servers (Git tools).
When you commit changes using terminal - remember to check terminal output to make sure
that no git hook failed

## Ensure you understand
When you work on a task ensure you understand exactly what you're expected to do.
Make sure you know what's the expected output and confirm you understand it properly.
Don't hesitate to ask if something's not clear. 

## Final notes
Before you proceed please confirm you already know about these rules.
Please write a message that confirms:

### how_to_commit.md
Already inlined above.

### chat_style.md
Use these rules when you talk to the user.
Don't use these rules when you create plan in file e.g. markdown.

**Message formatting**
Outlining, rich markdown and emojis help to structure the response. 
Always structure response to have distinguishable sections (ideally containing emojis) 
so one can read it in parts and quickly navigate to the part that's most interesting. 
Don't hesitate to use bold and italic to highlight key information. 
The goal is to make the response clear, easy to read and navigate.

**Main purpose - communicate crucial information**
The goal is to save time as much as possible.
Just tell what's the most important information one should know to understand your work.
Time is the most valuable resource.
Write it as shortly as possible.
Make it simple.

### code_quality.md
Always try to use latest packages and tools.
Keep an eye on code quality and readability.

Avoid writing big files.
Try to respect SOLID if it makes sense.
Readability counts.
If it makes sense - use TDD to write code.
Try to cover logic with tests.
Run tests to ensure everything works.

**Inspire with current code**
Use existing / surrounding code as reference.

### local_setup.md
**Delta**
I use Delta to render `git diff`.
Take a look https://github.com/dandavison/delta

**nvm**
If for any reason `yarn`, `pnpm`, `node` or whatever nvm-related doesn't work
then try to call `nvmrc-load` and then call the command again.

### show_used_rules.md
When user writes a message before responding write down:
- the rules you're using (rules that specify how you should respond etc)
- any other extra instructions you're following

Don't print the whole rules/instructions, just their names.
