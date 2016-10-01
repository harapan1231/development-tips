# development-tips

## Git

* Convert A Local repo to a remote one
git init
git add.
git commit -m "Initial commit"
git remote push add origin

* Delete file histories completely
git filter-branch --tree-filter 'command like rm -rf xxx' HEAD --all
git reflog expire --expire=now --all && git gc --aggressive --prune=now
git push --force origin master

* Check changed files
git ls-files --other --exclude-standard
