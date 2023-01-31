## can also do this from your command prompt, 
or open up bash or close git bash 
or open up a new terminal with command prompt
git init - be in the folder
# next steps:
git init - it will Initialize local a new repository, in the folder ur on
# opps it tends to be insible to see if your settings are not show hidden files
git status -shows what you have in you staging area
# it may ask , On branch main, No commits yet, Untracked files: (use "git add <file>..." to include in what will be committed)
## to options, if u ha muliple files u can spesify just a single on by running
git add <file> - adds files and folders to the staging area, file is the name
# or run
git add .
# this will add all files and folders to staging area
# u can alway run
git status
# before commiting to see erything is optimal
# or en open the file and add more to it if u want 
# remember to run git status to see if any files needs
git add .    to add all the changes u did again before commiting
git add
git commit -a
# once fornøyd 
git commit - commits files in staging area to local repository
# important to run now, whats in the "" does not really matter, depends on which branch is going tobe exported in github
# if u remember when creating a project in githud repo, it ask for which branch ""
# u can alway run
git status
# Changes to be committed:
git restore --staged <file>...
# Now that we added files to our staging area we 
# need to commit them to our local repository.
git commit -m “upload”
for instance 

git commit -m “upload”
or
# git push - Takes a local repository and pushes to a remote - - repository Github).
git push
    git remote add <name> <url>
and then push using the remote name
    git push <name>
# upload # main
git remote add upload "https://github.com/altlokalt/givencity.git"
git push upload
# if u dont ae an upstreamgit push --set-upstream upload main
# upload # main
git remote add main "https://github.com/altlokalt/givencity.git"
git push main -  'main' does not appear to be a git repository
fatal: Could not read from remote repository.
# myb the relation when u use git push
[main 90a513c] “upload”
 * [new branch]      main       -> upload/main
 * [new branch]      upload     -> upload/upload
# The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use
git push --set-upstream origin main
# To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote'

# Create a repo on github if u did not allerede 
set a remote Add your github credentials
git pull - Pull latest changes from remote repository
git clone - Clone repo from github

# u can skip this, since that is is default
git branch -M main

# Set remote by linking to repo url
git remote add origin <https://github.com/altlokalt/givencity.git>
# so run
git branch -M upload
git remote add origin "https://github.com/altlokalt/givencity.git"
git push -u origin main - to upload to github
# Now that all the files are set locally we are ready to push them to our remote repository. We set the remote so when we 
run git push
git knows which remote repo to send these files to.
# for EKS
git remote add origin https://github.com/altlokalt/givencity.git
# lastly
git push -u origin main
git push -u origin https://github.com/altlokalt/givencity.git
# tunnel access
https://vscode.dev/tunnel/DESKTOP-greg/c:/Users/grego



# Push to remote before sending to github
git pull - Pull latest changes from remote repository
# git push -u origin <branch name> FOR THIS EKS IS MASTER
git push -u origin main
git push -u origin upload
git pull ...
git pull <remote branch set> <branch in github>
git pull upload main
git pull upload givencity
If you wish to set tracking information for this branch you can do so with:
git branch --set-upstream-to=origin/<branch> main
# or whicher branch u spesify in github
# local branch first commit  githubs main
# if promted log in acess denien
git config user.name "new name"
git config credential.username "new name"
# eks
git config user.name "altlokalt"
# remove all GitHub entries from (Windows) Credential Manager
#Set useHttpPath = true in Git global configuration
git config --global credential.useHttpPath true
# You can validate this by checking
git config --global -e
# This will create a different entry for each user account.
# and create a file .gitconfig
#which u can sa or see by running git config --global -e
[filter "lfs"]
	clean = git-lfs clean -- %f
	smudge = git-lfs smudge -- %f
	process = git-lfs filter-process
	required = true
[user]
	name = altlokalt
	email = altlokalt@gmail.com
[credential]
	useHttpPath = true

# Testing your SSH connection which i tryied didnt work
git config user.name "altlokalt"

git config user.email "altlokalt@email.com"

eval $(ssh-agent -s)

ssh-add ~/.ssh/altlokalt.private

ssh -T git@github.com

git clone - Clone repo from github