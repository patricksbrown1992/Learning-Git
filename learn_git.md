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