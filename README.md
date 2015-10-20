<h2> Cheat Sheet </h2>

Whenever you're confused about git, come read this cheat sheet. Remember that all git commands can be run with the `--help` option. For example:

`$ git branch --help` or `$git log --help`

### Essential Git Commands

####Create a new git repository
`$ git init` - Create a new, local repository

#### Repo Status
`$ git status` - Check the status of your current repository and see which files have changed.

`$ git diff` - it compares two files and outputs the difference between them

#### Repo History
`$ git log` - it displays the logs of your commits with each commit ID, auther, date and message.

`$ git log --oneline --decorate --color --graph --all` - it displays the logs of your previous commits with color decorations and in one line only. 

`$ git log -p [filename]` Logs what happens in between commits

#### Stage files to commit
`$ git add <filename>` - Stages the file to be added to the repository

`$ git add -A` - Stages the current directory to be added to the repository

#### Commit changes in staged files
`$ git commit -m "<commit message>"` - Adds the staged file to the repository with a message describing the changes

#### Branching
`$ git branch <branch name>` - Creates a new local branch.

`$ git branch` - Shows the branches.

`$ git checkout <branch name>` - Switches to this branch.

#### Merging

`$ git merge <branch name>` - Merges this branch with the master

## Commands for working with a remote repository (e.g. Github)

`$ git clone <repo path or URL>` - clone a repository into a new directory.

`$ git remote` - List all remotes for the current repo.

`$ git remote add <remote name> <remote path or URL>` - adds a remote to your repo.

`$ git pull <remote name> <branch name>` - Pull down changes from a remote and integrate them into your repo. Performs `git fetch` and then `git merge`.

`$ git push <remote name> <branch name>` - Send your changes to the remote to be merged.


###Making Comman Lines Shortcuts
`git config --global alias` - this either sets up an alias for a specific command or create a whole new command. 

Example:
`git config --global alias.<the alias of your choice> <the original command>`
