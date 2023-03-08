# Git
So here's the deal, _git_ is a version control system that is basically a glorified save button.
Like the ones used in 8 bit games to save progress along the way. Anytime you fail a level, you can revert back to your saved checkpoint to restart.

I created this file as a mini note or as _cheatsheet_ to look back to.

# Git Setup
| Command | What it does |
|---------|--------------|
|`git config --global user.name "foo"`| Sets up a global username|
|`git config --global user.email "foo.bar@gmail.com"`| Sets up global mail|
|`git config --global init.defaultBranch main`| Changes the default branch for Git|
|`git config --global color.ui auto` | Colorful gitoutput for staging changes|
|`git config --global pull.rebase false`| Changes the default branch reconcilliation behavior|
|`git config --get user.name` | Fetches username used|
|`git config --get user.email`| Fetches the used mail|

# SSH Setup
| Command | What it does |
|---------|--------------|
|`ls ~/.ssh/id_ed25519.pub`| Checks to see if an SSH key is already installed |
|`ssh-keygen -t ed25519 -C <foo-email>`| Creats a new SSH key under the mail |
|`cat ~/.ssh/id_ed25519.pub`| Prints the public SSH key |
|`ssh -T git@github.com`| Attempts to SSH to GitHub |


# Git Usage
| Command | What it does |
|---------|--------------|
|`git clone <SSH-Link>`| Clones the repository to the current machine |
|`git remote -v`| Shows the URL of the repository created on GitHub |
|`git status`| Checks if any changes has been made to the files in the working directory |
|`git add .`| Adds all the file in the current directory to the staging area |
|`git commit -m "foo"`| Creates a commit to the main branch in the local machine |
|`git log`| Shows the modifications made to the branch by user and the time |
|`git push`<br>`git push origin main`| Pushes all the changes made to the remote repository |