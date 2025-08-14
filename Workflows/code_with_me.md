# code_with_me.md
Don't do many unrelated changes.
Do changes in small chunks and ask user to review them.

## Final notes
Before you proceed please confirm you already know about these rules.
Please write a message that confirms:

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
