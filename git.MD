GIT

## Config 

```
# Display all configuration values 
git config -l

# Set username and email
git config user.name "Dennie de Lange"
git config user.email "dennie@xxx.nl"
```

## Signing commits 

```
gpg --list-secret-keys --keyid-format LONG
git config --global user.signkey <signkey>
```

## SSH 

```
ssh-keygen -t rsa -b 4096 -C "dennie@xxx.nl"
```

https://www.atlassian.com/git/tutorials/atlassian-git-cheatsheet
  


Handige links:
* http://backlogtool.com/git-guide/en/
* http://git-scm.com/doc

Forking

Wijzigingen van geforked project terug mergen in je eigen clone:
@See:http://stackoverflow.com/questions/7244321/how-to-update-github-forked-repository
```
# Add the remote, call it "upstream":
git remote add upstream https://github.com/whoever/whatever.git

# Fetch all the branches of that remote into remote-tracking branches,
# such as upstream/master:

git fetch upstream

# Make sure that you're on your master branch:

git checkout master
# Rewrite your master branch so that any commits of yours that
# aren't already in upstream/master are replayed on top of that
# other branch:
git rebase upstream/master
```
* Checkout

|Omschrijving|Commando|
|------------|-----------|
|Remote checkout branch|git checkout -t origin/release-grails2|


# Git 

## Cheatsheet
 Command (after `git`) | Usage
--- | ---
`init` | Initialize directory as a git repository
`add .` | Add *all* untracked files to git 
`commit -am <message>` | Commit all pending changes using the message given.
`reset <commit>` | Resets the working tree to the specific commit, keeping uncommitted changes. 
`reset --hard <commit>` | Resets the working tree to specific commit and removing all uncommitted changes.   
`clean -f -d` | Remove untracked files
`checkout -b <branch>` | Checkout and switch to branch
`git log --pretty=oneline` | Show commit history

## One of 

You can target `one of` by using a `~`. If you want to target the previous commit,
you can use `HEAD~1`.   

## Relevant links:

Link | What
--- | --- 
https://git-scm.com/docs | Official documentation source
https://help.github.com/articles/ignoring-files/#create-a-global-gitignore | Setup global ignore file 