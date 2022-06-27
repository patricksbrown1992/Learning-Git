Learning Git
6-25-2022

Git Object Types-
    - Blob - files with extensions
    - Tree - stores info about directories
    - Commit - Store different versions
    - Annotated Tag - persisent text pointer to specific commit

git hash-object - create new files/blobs
git cat-file - see contents of file. has options. -p is print. -s is size. -t is type
git mktree - make new tree
stores object key as hash
hash has 2 to 160 power options
git read-tree hash_number

What is HEAD
    - Pointer to specific branch, to current checked out branch. Locally significant
Detached HEAD - points to specific commit instead of specific branch

fast forward merge- if you branch. Have new branch with changes and no new merges on master, it puts pointer on new branch
how to merge - go on main branch. Git merge feature_branch_name
3 way merge - main branch has other commits. Ancestor commit is last commit both branches have in common. Creates new merge commit at end of main branch that also points to end of feature branch. Then removes pointer on feature branch

Git fetch grabs updates from remote repo to local repo

git log has tags --oneline. lg. --graph. --stat
git shortlog - shows how many commits people have made

git reset. Has options --hard, --mixed, --soft

git revert HEAD

git amend - git commit --amend -m ""

git cherry-pick - want just one commit of another branch. automatically creates commit. Can do --no-commit

git reflog - reflog is an ordered list of the commits that HEAD has pointed to. git reflog show branch_name