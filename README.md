In this repo I keep my Cline Rules and Workflows I use every day.

# How to use
## MacOS
- Go to directory `~/Documents/Cline` (create it if not exist)
- `git clone git@github.com:Q-back/MyClineRules.git`

# work-notes
`work-notes` is a script that scaffolds the workflow with AI agent.
It's very simple and it just:
- creates `work-notes/` directory in current directory
- creates `work-notes/context/` directory
- creates `work_notes/prompt.md` file containing template for your prompt

### Create convenient symlinks for work-notes

For quick access you can create a `~/bin` directory (if it doesn't exist) 
and add two symbolic links pointing to the `work-notes` folder in this repo. 
One link uses the full name and the other a short alias.

Run these commands in your terminal (zsh):

```sh
# create ~/bin if missing
mkdir -p "$HOME/bin"

# create symlink named 'work-notes'
ln -s "$HOME/Documents/Cline/work-notes" "$HOME/bin/work-notes"

# create a second convenience symlink 'wn' pointing to the same target
ln -s "$HOME/Documents/Cline/work-notes" "$HOME/bin/wn"
```

Notes:
- If a link with the same name already exists, remove it first with 
`rm "$HOME/bin/work-notes"` or `rm "$HOME/bin/wn"`, or use `ln -sf` to overwrite.
- These are simple filesystem symlinks (no duplicate data). 
They just create shorter paths you can call from the shell or scripts.

### Ensure `~/bin` is on your PATH

Make sure your shell can find the new links by having `~/bin` in your `PATH`. 
For zsh you can add the following to `~/.zshrc` (if it's not already present):

```sh
echo 'export PATH="$HOME/bin:$PATH"' >> "$HOME/.zshrc"
source "$HOME/.zshrc"
```

If you use a different shell (bash, fish, etc.) add the equivalent entry to your shell's startup file.
