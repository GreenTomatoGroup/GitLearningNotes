# Git Learning Notes

## theory

SVN = 1 [remote] \(with all versions\) - N [local] 

Git = N [remote] - N[local] \(with all versions\)

Git has `branch` function

## Git Command

- init
- clone
- add (from unstaged to staged)
- commit
- push
- pull
- status

## from SVN to Git

- export svn repo
- new repo in gitlab 
- add .gitignore from [github](https://github.com/github/gitignore)
- add ReadMe.md
- git commit

## Commit - best practise

- first commit
- commit message: ACTION description
  - ADD, DELETE, UPDATE,  CHANGE, FIX...
  - JIRA#102 description
- don't combine multiple actions in one commit

## Branch

- represents an independent line of development
- You can think of them as a way to request a brand new working directory, staging area, and project history
- good for experimenting 

## Branch Merge

- combine 2 branches commits in to one branch

## Git flow

- manage branches systematically 
- develop: for development
- master: for production release
- feature: new feature, testing, new functions
- release: from develop to release, env. migration or bug fix
- hotfix: fix bugs on production, once finished, merge to master + develop

### Phase handling

- for new phase, open a new branch like `develop_phase1` for a copy of old phase, and keep develop a new phase on `develop`
- if you find a bug in old phase, fix it in `develop_phase1` branch.
- then check out current `develop` branch and merge `develop_phase1` fixes.

### Tag

- remark for important point in development
- e.g. build release
- Tag versioning
  - __major.minor.patch.buildnumber__
  - major: not backward compactible change
  - minor: backward compactible with a new feature
  - patch: bugfix
  - build number: each time build release
  - sync with mobile app version number

### ReadMe.md

- use of markdown
- markdown [cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
- Build configuration, api keys, structure, environment, remarks, etc...
- gitlab project page

### Gitlab 

- show gitlab interface
- how to add a new project
- how to name a project
- how to add project members